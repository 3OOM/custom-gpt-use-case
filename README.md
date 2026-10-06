# Topic 1 Assessment — Introduction to Custom GPTs: Use Case Definition

**Course Topic:** Topic 1 — Introduction to Custom GPTs: Use Case Definition  
**Student Name:** Abhishek Nikam  
**Repository:** `custom-gpt-use-case`  
**GitHub Link:** https://github.com/3OOM/custom-gpt-use-case  

---

## 📌 Project Overview

This repository contains the complete assessment deliverables for **Topic 1 — Introduction to Custom GPTs: Use Case Definition**. The project demonstrates the end-to-end workflow of identifying a high-frequency, recurring real-world problem within enterprise B2B ERP implementations and scoping it into an executive-grade Custom GPT use case document.

### Selected Use Case
* **GPT Name:** `OnboardIQ: ERP Integration Copilot`
* **Domain:** Enterprise Cloud ERP Systems Integration & Consulting
* **Purpose:** Automate and guide technical prerequisite gathering, API authentication validation, and data schema intake for client implementations, collapsing project kickoff lead times from 11 days to under 4 days.

---

## 📁 Repository Structure

```
custom-gpt-use-case/
├── README.md                 # Complete project documentation, LMS copy-paste text, video script
├── use_case_document.md      # Mandatory 1-page Use Case Document (Core Deliverable)
└── supporting_notes.md       # Brainstorming matrix, ChatGPT prompt logs, and feasibility validation
```

---

## 📄 Key Deliverables Manifest

| Deliverable File | Type | Description |
|---|---|---|
| [`use_case_document.md`](use_case_document.md) | **Mandatory** | The official 1-page use case definition document covering **GPT Name**, **Target Users (Primary & Secondary)**, **Problem Statement (Cause, Impact, Current Gap)**, **Expected Outcomes (Measurable)**, and **Clarity, Relevance, Feasibility Validation**. |
| [`supporting_notes.md`](supporting_notes.md) | **Supporting** | Comprehensive documentation of candidate problem trade-offs, ChatGPT naming brainstorm logs, prompt refinement iterations, user persona diagrams, and Custom GPT architectural feasibility mapping. |
| [`README.md`](README.md) | **Guide** | Project overview, assessment checklist verification, LMS submission description copy, and 3-minute Loom video presentation script. |

---

## 📋 Copy-Paste LMS Submission Details

When submitting in the LMS, copy and paste the following text into the respective submission fields:

### 1. Description Field Submission Text

```markdown
### Topic 1 Assessment: Introduction to Custom GPTs — Use Case Definition

**GPT Name:** OnboardIQ: ERP Integration Copilot
**Repository URL:** https://github.com/3OOM/custom-gpt-use-case
**Deliverable File:** use_case_document.md

#### 1. Challenges Faced in Narrowing the Problem & Resolutions
- **Challenge:** Initially, the problem statement spanned the entire multi-month ERP implementation lifecycle (including user training and go-live hypercare), which was overly broad for a single Custom GPT.
- **Resolution:** Scoped the GPT specifically to the high-friction "Technical Intake & Prerequisite Gathering" phase (Kickoff Days 1–14). This established a crisp boundary: API credential intake, endpoint parameter validation, and data migration CSV schema checking.

#### 2. Key Assumptions Made About Target Users
- **Primary Users:** Client technical leads are assumed to have basic familiarization with their source systems (e.g., existing CRM or database) but lack in-depth familiarity with the target ERP's exact REST API formats, webhook protocols, or chart-of-accounts schema.
- **Consultants:** Associate implementation consultants possess domain knowledge but spend excessive hours re-explaining the same checklist prerequisites across disparate email threads.

#### 3. Alternative Use Cases Considered & Why Deprioritized
- **Alternative 1 (Internal Corporate IT Tier-1 Helpdesk):** While ticket volume was high (30–40/day), resolution frequently required direct write access to enterprise identity providers (Active Directory / Okta), which exceeds standard Custom GPT out-of-the-box knowledge retrieval.
- **Alternative 2 (Security RFP & Compliance Questionnaire Assistant):** Addressed a lower monthly frequency (5–8/month) and offered less interactive conversational engagement than client onboarding.
- **Selection Decision:** The Client ERP Onboarding Copilot offered the highest frequency (15–20 engagements/quarter), clear structured input requirements, and high feasibility using standard Custom GPT capabilities (Knowledge retrieval + Custom Instructions + Code Interpreter for CSV schema validation).
```

### 2. Video Demonstration Link
* **Loom / YouTube Link:** `https://www.loom.com/share/custom-gpt-use-case-walkthrough` *(Replace with your recorded video URL)*

---

## 🎥 Video Demonstration Script (3-Minute Loom / YouTube Guide)

Follow this structured script when recording your assessment walkthrough video:

| Timestamp | Section | Talking Points / Visual Demonstration |
|---|---|---|
| **0:00 – 0:40** | **Introduction & Problem Identification** | • Show GitHub repository `custom-gpt-use-case`.<br>• Introduce yourself: *"Hello, I am Abhishek Nikam, presenting Topic 1: Custom GPT Use Case Definition."*<br>• Explain the real-world problem: During ERP implementations, client onboarding stalls due to confusing technical prerequisite questionnaires, delaying kickoff by 11 days. |
| **0:41 – 1:20** | **GPT Name & Target Users** | • Navigate to `use_case_document.md`.<br>• Highlight the name **OnboardIQ: ERP Integration Copilot** and explain the naming rationale.<br>• Walk through **Primary Users** (Client Tech Leads & Associate Consultants) and **Secondary Users** (Senior Architects & PMs). |
| **1:21 – 2:10** | **Problem Statement & Expected Outcomes** | • Read the refined Problem Statement highlighting Root Cause, Impact, and Current Gap.<br>• Present the 4 measurable outcomes: 60% intake time reduction, 70% fewer clarification emails, 90%+ first-pass spec completeness, and 4.5 billable hours saved per project. |
| **2:11 – 3:00** | **Validation Matrix & Conclusion** | • Show the Validation Matrix scoring 5/5 across Clarity, Relevance, and Feasibility.<br>• Briefly show `supporting_notes.md` displaying the ChatGPT naming brainstorm and candidate problem evaluation.<br>• Conclude with LMS readiness and GitHub commit status. |

---

## ✅ Practical Assessment Checklist Verification

| Requirement / Task Description | Status | Verification Reference |
|---|:---:|---|
| Real-world problem identified and documented | **PASS** | `use_case_document.md` (Section: Problem Statement) & `supporting_notes.md` |
| GPT Name defined and descriptive | **PASS** | `OnboardIQ: ERP Integration Copilot` (`use_case_document.md`) |
| Target Users (primary/secondary) clearly defined | **PASS** | `use_case_document.md` (Section: Target Users) |
| Problem Statement is specific and grounded | **PASS** | Covers Cause, Impact, and Current Gap (`use_case_document.md`) |
| Expected Outcomes are measurable | **PASS** | 4 quantifiable targets with % and hour metrics |
| Use case validated against Clarity, Relevance, Feasibility | **PASS** | Validation Matrix in `use_case_document.md` |
| Use case document is approximately one page | **PASS** | Verified concise one-page layout |
| Final document saved as `use_case_document.md` | **PASS** | Located in repository root |
| Repository uploaded to GitHub | **PASS** | Committed and pushed to `https://github.com/3OOM/custom-gpt-use-case` |
