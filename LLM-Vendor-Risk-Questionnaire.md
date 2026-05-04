# LLM Vendor Risk Assessment Questionnaire
**Purpose**: Third-Party Risk Management (TPRM) for OpenAI, Anthropic, Azure OpenAI, AWS Bedrock, Google
**Frameworks**: NIST AI RMF, ISO/IEC 42001, SOC 2, FedRAMP, EU AI Act

## Instructions to Vendor
Provide evidence for each. “N/A” requires justification. <80% compliance = High Risk.

### Section 1: Data Governance & Privacy
1. Is customer prompt/completion data used to train your foundation models? Provide opt-out documentation.
2. Data retention period for prompts, completions, embeddings? Can customer configure zero-day retention?
3. Is data encrypted at rest AES-256 and in transit TLS 1.2+? Provide architecture diagram.
4. Geographic location of data processing/storage? List all countries. FedRAMP Moderate/High regions?
5. Do you offer Business Associate Agreement (BAA) for HIPAA? Provide template.
6. Provide current SOC 2 Type II and ISO/IEC 42001 certificates. Date of last audit?

### Section 2: Model Risk & LLM Security
7. Describe tenant isolation architecture. How is Customer A data segregated from Customer B?
8. Do you conduct adversarial red-teaming for prompt injection, jailbreaking, training data extraction, model inversion? Frequency? Share latest summary report.
9. List all subprocessors with access to customer data. Location and purpose.
10. Content filtering capabilities: PII detection, toxicity, code injection. Can customer tune filters?
11. Describe incident response process for model data leakage. Customer notification SLA?

### Section 3: Compliance & Transparency
12. How do you comply with EU AI Act for high-risk AI systems? Provide conformity assessment.
13. Are model cards and data cards available per Google/IBM standards? Provide links.
14. Can customers disable human review/logging of prompts for privacy-sensitive workloads?
15. Data Processing Addendum (DPA) available? Includes SCCs for international transfer?

### Section 4: Contractual
16. Liability for IP infringement from model outputs? Indemnification provided?
17. Right to audit clause included? Penetration test reports available under NDA?
18. Exit strategy: How is data returned/deleted at contract termination? Provide certification.

**Scoring**: Critical = Q1,2,4,5,7,16. Any “No” on Critical = Automatic High Risk.
