# Supporting Notes & Brainstorming Artifacts

**Topic 1 — Assessment: Introduction to Custom GPTs: Use Case Definition**  
**Project:** OnboardIQ: ERP Integration Copilot  
**Author:** Abhishek Nikam  
**Target Repository:** `custom-gpt-use-case`  

---

## 1. Candidate Problems Evaluation (Exercise 1)

To identify the most viable, high-impact use case for a Custom GPT, three recurring operational bottlenecks were analyzed across frequency, clarity, feasibility, and business impact.

| Candidate Problem | Domain / Operational Context | Recurring Frequency | Clarity & Scope | Custom GPT Feasibility | Selected? |
|---|---|:---:|:---:|:---:|:---:|
| **Option A: Client ERP Integration & Technical Prerequisite Onboarding** | B2B Enterprise ERP Consulting & Systems Integration | High (15–20 new client kickoffs / quarter) | High: Discrete technical checklists (APIs, schemas, tokens, chart of accounts) | **High**: Standard Custom GPT with Knowledge docs and structured system prompts | **SELECTED** |
| **Option B: Internal IT Tier-1 Helpdesk & Access Provisioning** | Internal Corporate IT Operations | Very High (30–40 tickets / day) | Moderate: Broad variety of internal hardware/software inquiries | **Moderate**: Many actions require direct Active Directory / Okta write API integrations | Discarded |
| **Option C: Security RFP & Compliance Questionnaire Responder** | Sales Engineering & Bid Management | Low-Medium (5–8 RFPs / month) | High: Questionnaires mapped to SOC2 / ISO policies | **Moderate-High**: Requires huge knowledge library; low conversational interactivity | Discarded |

### Selection Rationale
* **Why Option A was chosen:** Client ERP onboarding is a high-friction, mission-critical workflow with recurring, structured information exchange. Technical prerequisite gathering is conversational by nature (clarifying endpoints, explaining token formats, validating CSV schemas), which directly matches the strengths of a Custom GPT's conversational reasoning and knowledge file retrieval capabilities.
* **Why Options B & C were deprioritized:** Option B frequently requires backend write actions (e.g., password reset scripts, ticket resolution triggers) which exceed a pure Topic 1 Custom GPT use case. Option C offers lower frequency and less interactive engagement.

---

## 2. GPT Naming Brainstorming & Selection (Exercise 2)

### Prompt Executed in ChatGPT
```text
Act as a senior product marketing manager and AI solutions architect.
I am developing an enterprise Custom GPT designed to assist client implementation leads and consultants during the initial technical onboarding and API/prerequisite gathering stage of an ERP implementation.

Generate 5 distinct candidate names that:
1. Clearly communicate its purpose (onboarding + ERP technical prerequisites).
2. Sound professional and enterprise-grade.
3. Are concise, memorable, and avoid generic labels like "AI Bot".

For each name, provide a 1-sentence rationale and score it for clarity.
```

### Brainstorming Results & Evaluation

| Candidate Name | Style / Theme | Evaluation & Feedback | Score (1–10) | Status |
|---|---|---|:---:|:---:|
| 1. **ERP OnboardBot** | Descriptive | Functional, but sounds dated and mechanical; lacks enterprise consulting prestige. | 6/10 | Rejected |
| 2. **Integration Kickoff Navigator** | Action-oriented | Clear scope, but omits the key domain keyword "ERP". | 7/10 | Rejected |
| 3. **OnboardIQ: ERP Integration Copilot** | Professional / Enterprise | Combines brand identity ("OnboardIQ") with explicit domain context and modern AI terminology ("Copilot"). | **9.8/10** | **SELECTED** |
| 4. **ERP Implementation Prerequisite Guide** | Literal / Functional | Accurate, but overly verbose and lacks conversational branding. | 7.5/10 | Rejected |
| 5. **ClientTech Onboarder** | Modern SaaS | Punchy, but too informal for executive IT stakeholders. | 7/10 | Rejected |

**Selected Winner:** `OnboardIQ: ERP Integration Copilot`

---

## 3. Problem Statement Drafting & Refinement (Exercise 3)

### Initial Raw Draft
> *"Clients taking on our ERP implementation take way too long to fill out technical questionnaires. They don't know what API credentials or webhook URLs to provide, so consultants have to send dozens of emails back and forth. This delays the kickoff and costs us lots of wasted consulting hours."*

### ChatGPT Refinement Prompt
```text
Act as a management consultant specializing in business process optimization.
Review the following draft problem statement for an enterprise Custom GPT use case.
Refine it into a concise, professional 2 to 3 sentence problem statement that explicitly highlights:
1. Root Cause: What causes the bottleneck?
2. Impact: Measurable business friction (schedule delays, consulting overhead).
3. Current Gap: Why existing manual methods (emails, spreadsheets) fail.

Ensure the tone is objective, precise, and executive-ready.
```

### Final Refined Problem Statement
> *"During B2B ERP system implementations, client onboarding frequently stalls because non-technical client stakeholders are overwhelmed by complex technical prerequisite questionnaires (encompassing API endpoints, webhook security, ledger mappings, and data migration schemas). Currently, this gap forces implementation consultants to conduct 4 to 6 rounds of ad-hoc email exchanges and manual spreadsheet reviews, delaying project kickoffs by an average of 11 business days, increasing unbilled consulting overhead, and causing early-stage client friction."*

---

## 4. Target User Personas & Context

```
+-----------------------------------------------------------------------------------+
|                              TARGET USER ECOSYSTEM                                 |
+-----------------------------------------------------------------------------------+
|                                                                                   |
|   PRIMARY USERS (Active Conversationalists)                                       |
|   +---------------------------------------+   +--------------------------------+  |
|   | Client Technical Leads & POCs         |   | Associate Implementation Team  |  |
|   | - Submits API credentials & scopes    |   | - Reviews submitted specs      |  |
|   | - Clarifies ERP data mapping rules    |   | - Runs checklist validation    |  |
|   | - Troubleshoots sandbox connectivity  |   | - Tracks onboarding milestones |  |
|   +---------------------------------------+   +--------------------------------+  |
|                                                                                   |
|                                         │ (Feeds structured outputs to)           |
|                                         ▼                                         |
|                                                                                   |
|   SECONDARY USERS (Beneficiaries)                                                 |
|   +---------------------------------------+   +--------------------------------+  |
|   | Senior Solution Architects            |   | Project Managers (PMs)         |  |
|   | - Receives clean, pre-validated specs |   | - On-time kickoff assurance    |  |
|   | - Focuses on core systems design      |   | - Predictable delivery margins |  |
|   +---------------------------------------+   +--------------------------------+  |
+-----------------------------------------------------------------------------------+
```

---

## 5. Feasibility Validation & Implementation Readiness (Exercise 4)

### Capability Mapping to Standard Custom GPT Features
* **Custom Instructions (System Persona):** Governs conversational pacing, asks one intake domain at a time (Authentication -> Endpoints -> Data Schemas -> Webhooks), and provides schema validation rules.
* **Knowledge Files:** Upload standard ERP integration guidebooks, REST/SOAP API checklist templates, and sample CSV data migration templates.
* **Conversation Starters:**
  1. *"Start ERP technical onboarding checklist for a new client"*
  2. *"Validate my API endpoint security parameters"*
  3. *"Explain chart-of-accounts CSV format requirements"*
  4. *"Generate onboarding summary report for the Solution Architect"*
* **Capabilities Enabled:** Web Browsing (for checking standard ERP API documentation) and Code Interpreter (for validating client CSV data schemas).
