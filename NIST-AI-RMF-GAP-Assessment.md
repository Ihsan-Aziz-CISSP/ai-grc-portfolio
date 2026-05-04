# NIST AI RMF 1.0 GAP Assessment Template
**Use Case**: Enterprise GenAI Rollout – ChatGPT Enterprise + Azure OpenAI
**Version**: 1.0 | **Date**: Oct 2026

## How to Use
Score each sub-category: 0=Not Implemented, 1=Partial, 2=Mostly, 3=Fully Implemented. <70% = High Risk.

## GOVERN Function
| ID | Sub-Category | Current State | Score | Gaps | Remediation | Owner | Due | 800-53 Map |
| --- | --- | --- |
| GOVERN 1.1 | AI policies are in place | AI AUP drafted, not approved | 1 | Legal review pending | Legal sign-off | CISO | 11/15/26 | PL-1, PL-4 |
| GOVERN 1.2 | Accountability structures | AI Council formed | 2 | RACI unclear | Publish RACI | CIO | 10/30/26 | PM-2 |
| GOVERN 2.1 | Risk tolerances defined | General risk appetite only | 0 | No AI-specific tolerance | Define AI risk tolerance | CRO | 11/30/26 | RA-3 |

## MAP Function
| ID | Sub-Category | Current State | Score | Gaps | Remediation | Owner | Due |
| --- | --- | --- | --- |
| MAP 1.1 | Intended purpose defined | Use cases documented | 2 | Impact assessment missing | Complete AIA | PO | 11/1/26 |
| MAP 2.3 | AI risks identified | Ad-hoc only | 1 | No formal risk register | Build AI Risk Register | ISSO | 10/20/26 |

## MEASURE Function
| ID | Sub-Category | Current State | Score | Gaps | Remediation | Owner | Due |
| --- | --- | --- | --- |
| MEASURE 2.11 | Regular testing | None | 0 | No red-team | Schedule quarterly LLM pen test | AppSec | 12/1/26 |

## MANAGE Function
| ID | Sub-Category | Current State | Score | Gaps | Remediation | Owner | Due |
| --- | --- | --- | --- |
| MANAGE 4.1 | Post-deployment monitoring | Basic logging | 1 | No bias/drift monitoring | Deploy LangSmith + evals | MLOps | 12/15/26 |

**Summary Score**: 45% – High Risk. Remediation plan tracked in POA&M tab.

*Full Excel version with formulas and 800-53 crosswalk available on request.*
