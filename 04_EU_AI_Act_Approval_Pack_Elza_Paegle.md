# EU AI Act Approval Pack

**Consultant:** Elza Paegle  
**Client cases reviewed:** Photography studio, social media agency, hair-salon chain and pole dance studio

## Executive Summary

The four proposals represent all four EU AI Act outcomes. The photography-selection system is minimal risk and can be approved. The social media assistant mainly triggers Article 50 transparency obligations and can proceed with controls. The recruitment system is high-risk under Annex III and requires a complete compliance and human-oversight framework before deployment. The workplace emotion-recognition system is prohibited and must be denied and redesigned.

The overall recommendation is therefore one approval, two conditional approvals and one denial with a lawful alternative.

## Case A — Photography Studio

**Client request:** The studio wants AI to analyse photographs for technical quality, closed eyes, duplicates, composition and sharpness and then propose a delivery gallery.

**Classification:** Minimal risk.

**Architecture and human oversight:** Images from a completed shoot enter a technical-quality and similarity model. The model creates a suggested gallery, but the photographer reviews every selection and can remove or restore photographs before delivery. The system should record the model version and the photographer’s final selection.

**Role map:** The photo-software vendor is the provider; the photographer or studio is the deployer; cloud storage or computer-vision companies may be third-party vendors.

**Compliance implications:** No specific high-risk AI Act obligations apply. GDPR, confidentiality and intellectual-property requirements remain relevant. The studio should use secure storage, retention limits and appropriate client information. Images should not be reused for facial recognition or model training without an appropriate legal basis.

**Decision: Approve.**

**Operational artifact:** Image handling and retention policy.

## Case B — Social Media Agency

**Client request:** The agency wants a conversational assistant that answers clients’ questions and generates content ideas, captions and posting suggestions.

**Classification:** Limited risk with transparency obligations.

**Architecture and human oversight:** A client question and approved business information trigger the model. The assistant generates a draft response, which the client reviews. Clients can escalate to a human social media manager. The interface should display an AI disclosure and retain appropriate records of model versions, outputs and escalations.

**Role map:** The assistant vendor is the provider, although the agency may become the provider if it develops or offers the system under its own name. The agency is the deployer, and the general-purpose model and hosting companies are third-party vendors.

**Compliance implications:** Clients must be informed that they are interacting with AI. The agency should provide human escalation, privacy information, content checks and safe-use boundaries. Outputs should not be represented as verified legal, medical or financial advice. Synthetic-content marking should be supported where applicable.

**Decision: Approve with controls.**

**Operational artifact:** AI transparency notice and escalation procedure.

## Case C — Hair-Salon Recruitment

**Client request:** The salon chain wants AI to score applicants using their CVs, portfolios, training records and application answers and recommend who receives an interview.

**Classification:** High-risk under Annex III because the system analyses, filters and evaluates candidates for employment.

**Architecture and human oversight:** Application materials enter a recruitment model that produces a suitability score and interview recommendation. A trained recruiter must independently examine the evidence rather than automatically accepting the ranking. Inputs, scores, overrides, model versions and final decisions must be logged.

**Role map:** The recruitment-AI vendor is the provider; the salon chain is the deployer; applicant-tracking, cloud and model companies may be third-party vendors.

**Compliance implications:** Deployment depends on risk management, appropriate data governance, bias testing, technical documentation, automatic logging, transparency, meaningful human oversight, accuracy, robustness and cybersecurity. The provider must address conformity assessment and applicable registration requirements. The salon must monitor operation, retain relevant logs, inform applicants and ensure reviewers have the competence and authority to override the system. GDPR profiling and DPIA requirements should also be assessed.

**Decision: Approve with controls. Launch is conditional on completing the high-risk compliance framework.**

**Operational artifact:** Risk-management file, candidate notice and bias-testing protocol.

## Case D — Pole Dance Studio

**Client request:** The studio wants cameras and AI to infer instructors’ enthusiasm, frustration, confidence and stress and produce weekly individual “classroom energy” scores.

**Classification:** Prohibited. Article 5 prohibits AI emotion inference in the workplace unless a narrow medical or safety exception applies. No such exception is present. Human review does not make the system lawful.

**Architecture and role map:** The proposed system would send video and audio to an emotion-analysis model and provide individual scores to management. The emotion-analysis vendor would be the provider and the studio the deployer. This architecture must not be launched.

**Compliance implications:** The studio should stop procurement and avoid collecting facial or voice data for emotion inference. It should document the rejection and consult staff before introducing any alternative monitoring process.

**Decision: Deny and redesign.**

### Lawful redesign

Remove emotion inference and individual psychological scoring. Collect voluntary and anonymous student feedback about observable matters such as instructional clarity, safety guidance and respectful conduct. AI may summarise aggregated, non-identifying studio-level feedback, but it should not infer emotions or recommend employment actions. Managers should conduct human observations using documented behavioural and safety criteria.

**Operational artifact:** Prohibited-use decision and lawful redesign specification.

## Overall Sign-off

| Case | Category | Decision |
|---|---|---|
| A — Photography studio | Minimal risk | Approve |
| B — Social media agency | Limited risk / transparency | Approve with controls |
| C — Hair salon | High-risk | Approve with controls |
| D — Pole dance studio | Prohibited | Deny and redesign |

## What Changed After the Client Discussion?


The partner revealed that the intended categories were Case A — minimal risk, Case B — limited risk with transparency obligations, Case C — high-risk and Case D — prohibited. All four intended categories matched the independent consulting classifications.

The partner accepted the recommendations. During the discussion, we clarified that human review does not remove the high-risk classification of the recruitment system and cannot make workplace emotion inference lawful. The final recommendation did not change. The redesign of Case D was retained: emotion inference and individual energy scores would be removed and replaced with voluntary feedback and human observation based on transparent behavioural and safety criteria.

## References

- [Regulation (EU) 2024/1689 — EU Artificial Intelligence Act](https://eur-lex.europa.eu/eli/reg/2024/1689/oj/eng)
- [European Commission — AI Act regulatory framework](https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai)
