# Consulting Review of Partner Cases

**Consultant:** Elza Paegle  
**Purpose:** Independent first-pass classification completed without seeing the partner’s private answer key.

| Case | Likely category | Why this is the first-pass call | Proposed AI architecture | Provider / deployer / vendor | Required obligations or controls | Decision |
|---|---|---|---|---|---|---|
| A — Photography studio | Minimal risk | The system assists with technical photo selection and does not determine access to employment, education, services or another Annex III area. The photographer retains the final decision. | Completed shoot triggers analysis of photographs and metadata. The model detects blur, closed eyes, duplicates, composition and sharpness. It produces a suggested gallery. The photographer reviews, removes or restores images. The system records the model version and accepted or rejected suggestions. | Provider: photo-selection software vendor. Deployer: photography studio or photographer. Third parties: cloud storage, hosting or computer-vision providers. | No case-specific high-risk obligations. Apply GDPR controls, secure storage, retention limits, client information and human review. Do not repurpose photographs for facial identification or model training without an appropriate legal basis. | **Approve** |
| B — Social media agency | Limited risk / transparency | Clients interact directly with an AI assistant through a chat interface. Article 50 transparency applies even though clients can escalate to a human manager. | A client question and approved business information trigger the assistant. The model retrieves relevant business context and generates a draft caption, idea or posting recommendation. The client reviews the output or escalates to a human manager. The interface displays an AI disclosure and records the model version, prompt, output and escalation. | Provider: assistant vendor, or the agency if it develops and offers the system under its own name. Deployer: social media agency. Third parties: general-purpose AI model, hosting and analytics providers. | Clearly disclose that the client is interacting with AI. Provide human escalation, output review, privacy controls, content-safety checks and records of important interactions. Generated content should not be presented as verified professional advice. Relevant synthetic-content marking should be supported where applicable. | **Approve with controls** |
| C — Hair salon | High-risk | The system analyses, scores and filters applicants and recommends who receives an interview. Recruitment and candidate evaluation are Annex III high-risk uses. A manager’s ability to override the score does not remove the classification. | An application triggers analysis of CVs, portfolios, training and answers. The model produces a suitability score and interview recommendation. A trained recruiter independently reviews the evidence and can reject the recommendation. The system logs inputs, scores, overrides, model version and final decisions. | Provider: recruitment-AI vendor. Deployer: salon chain. Third parties: applicant-tracking, cloud or model providers. The salon could become the provider if it substantially modifies or markets the system under its own name. | Require risk management, representative data, bias testing, technical documentation, automatic logs, transparency, human oversight, accuracy, robustness and cybersecurity. The provider must address conformity assessment and registration requirements. The salon must monitor use, retain relevant logs, inform applicants and ensure reviewers are trained and able to override the system. GDPR profiling and DPIA requirements should also be assessed. | **Approve with controls** |
| D — Pole dance studio | Prohibited | The system infers instructors’ emotions from facial expressions and voices in their workplace. Article 5 prohibits workplace emotion inference except for narrowly defined medical or safety purposes. Management review does not make the practice lawful. | Proposed design: cameras and microphones capture lessons; a model infers enthusiasm, frustration, confidence and stress; instructors receive individual scores; management reviews the dashboard. Because the intended use is prohibited, this architecture must not be deployed. | Provider: emotion-analysis vendor. Deployer: pole dance studio. Third parties: camera, cloud-hosting or model providers. Both placing such a system on the market for this purpose and using it create compliance concerns. | Stop procurement and deployment. Do not collect facial or voice data for emotion inference. Remove emotional-state predictions and individual “energy” scores. Complete privacy and workplace consultation before adopting any alternative monitoring process. | **Deny and redesign** |

## Lawful Redesign of Case D

The studio should remove facial, voice and behavioural emotion inference entirely. Students could instead provide voluntary, anonymous feedback about observable class features, such as whether instructions were clear, safety guidance was followed and participants were treated respectfully.

AI could summarise aggregated, non-identifying feedback at studio level, but it should not infer instructors’ emotions, create individual psychological profiles or automatically recommend scheduling and employment actions. Managers should conduct periodic human observations against documented behavioural and safety criteria and discuss the results directly with instructors.

## Borderline Considerations

- **Case A:** The classification could change if facial identification, biometric categorisation or client profiling were added. GDPR still applies to identifiable photographs.
- **Case B:** Human escalation does not remove Article 50 transparency. Additional disclosure may be needed if generated material concerns matters of public interest.
- **Case C:** Human review does not remove high-risk status when the system’s intended purpose is to score and filter candidates.
- **Case D:** Calling the output a “classroom energy” or “wellbeing” score does not change the fact that the system infers emotions in a workplace.

## Recommended Next Operational Artifacts

- **Case A:** Image handling and retention policy.
- **Case B:** AI transparency notice and human-escalation procedure.
- **Case C:** Risk-management file, candidate notice and bias-testing protocol.
- **Case D:** Written prohibited-use decision and lawful redesign specification.

## References

- [Regulation (EU) 2024/1689 — EU Artificial Intelligence Act](https://eur-lex.europa.eu/eli/reg/2024/1689/oj/eng)
- [European Commission — AI Act regulatory framework](https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai)
