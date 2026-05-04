# AI Acceptable Use Policy – Enterprise Template
**Version**: 1.0 | **Owner**: Information Security GRC | **Date**: Oct 2026
**Frameworks**: NIST AI RMF 1.0, ISO/IEC 42001, OWASP Top 10 for LLMs, EU AI Act, HIPAA

## 1. Purpose
This policy establishes requirements for secure use of Generative AI and Large Language Models (LLMs) including ChatGPT Enterprise, Azure OpenAI Service, AWS Bedrock, and Google Vertex AI. Objective: enable AI innovation while preventing data leakage, IP loss, model bias, and regulatory non-compliance.

## 2. Scope
Applies to all employees, contractors, vendors, and third parties with access to company systems or data.

## 3. Approved AI Tools Only
| Tool | Status | Data Controls |
| --- | --- | --- |
| ChatGPT Enterprise | Approved | Zero data retention, SOC 2, SSO enabled |
| Azure OpenAI | Approved | Private network, content filtering, no human review |
| AWS Bedrock | Approved | VPC only, encryption at rest |
| Public ChatGPT, Claude.ai, Bard, Perplexity | Prohibited | No enterprise controls |

## 4. Prohibited Data – Never Input Into Any LLM
- **PII**: SSN, DOB, driver’s license, financial account numbers
- **PHI**: Patient names, medical records, diagnosis, treatment data per HIPAA
- **PCI**: Credit card numbers, CVV, magnetic stripe data
- **Confidential IP**: Source code, trade secrets, unreleased financials, M&A data, strategic plans
- **Customer Data**: Any client data not approved by Legal/Privacy for AI processing
- **Credentials**: API keys, passwords, tokens, certificates

## 5. Prompt Injection & LLM Security Controls
Users must not attempt to bypass safety controls via jailbreaks, DAN prompts, or roleplay attacks. All prompts are logged per NIST AI RMF *Measure* function. Security uses DLP + CASB to detect PII/PHI in prompts.

## 6. AI Output Validation Requirements
LLM outputs may contain hallucinations or bias. Human review is mandatory before:
1. External client communication
2. Code deployment to production
3. Decisions impacting hiring, lending, healthcare, or legal matters per EU AI Act

All AI-generated content must include disclaimer: “Drafted with AI assistance and reviewed by [Name]”

## 7. Training & Attestation
Annual “Safe Prompting for GenAI” training required. Covers data classification, prompt injection, and incident reporting. 100% attestation required for access.

## 8. Incident Reporting
Suspected PII/PHI leakage, prompt injection success, or AI misuse → report to `security@company.com` within 1 hour per Incident Response Plan.

## 9. Violations
Violations may result in loss of AI access, disciplinary action up to termination, and legal action.

**Control Mapping**: NIST AI RMF Govern 1.1, Map 2.3, Measure 2.11 | ISO/IEC 42001 8.2, 8.3 | NIST 800-53 Rev.5 PL-4, PT-2, SA-22, SI-10
