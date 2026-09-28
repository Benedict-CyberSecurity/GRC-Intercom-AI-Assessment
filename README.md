# Intercom Fin AI Agent — Third-Party Risk & AI Governance Assessment

**Author:** Eliza Benedict  
**Client:** Island Shores Artisans & Tours (Simulated Case Study)  
**Location:** Charlottetown, Prince Edward Island (PEI), Canada  
**Date:** September 2026  
**Frameworks:** ISO 27001:2022 | ISO 42001 (AI Management) | NIST AI RMF 1.0 | PIPEDA | GDPR  

---

## Portfolio Repository Overview

This repository contains a comprehensive **Third-Party Risk Management (TPRM) and AI Governance Assessment** evaluating the integration of the **Intercom Fin AI Agent** for a simulated business scenario (*Island Shores Artisans & Tours*). 

The goal of this project is to demonstrate practical, client-ready GRC consulting capabilities—moving beyond vendor SOC 2 certificates to establish actionable customer-side controls, data lineage mapping, and operational Standard Operating Procedures (SOPs).

---

## Repository Structure

```text
grc-intercom-ai-assessment/
│
├── README.md                           <-- Master Portfolio Landing Page & Assessment Report
├── grc-intercom-project.docx           <-- Downloadable Word Document (Editable / Executive PDF)
│
└── sops/
    ├── SOP-001-DSAR-Playbook.md        <-- Operational Privacy Playbook (PIPEDA / GDPR 30-Day SLA)
    ├── SOP-002-RAG-Governance.md       <-- AI Knowledge Base Governance & Adversarial Testing
    └── SOP-003-TPRM-Monitoring.md      <-- Continuous Subprocessor & Vendor Risk Procedure
```

---

## Deliverables & GRC Competencies Summary

| Deliverable / Section | GRC Capability Demonstrated |
| :--- | :--- |
| **Executive Dashboard & Remediation Matrix** | Executive Stakeholder Communication & Prioritised Risk Reporting |
| **Scope, Methodology & Evidence Framework** | Formal Assessment Framework, Evidence Classification & Scope Boundary |
| **System Architecture & Data-Flow Map** | Third-Party Data Flow Mapping, Subprocessor Analysis & Shared Responsibility |
| **Control Assessment Matrix** | ISO 27001, ISO 42001 & NIST AI RMF Control Mapping & Gap Analysis |
| **Privacy & Regulatory Assessment** | PIPEDA / GDPR Cross-Border Data Transfer, Transparency & Minimisation Analysis |
| **Risk Register & Scoring Methodology** | Qualitative Risk Analysis (Inherent vs. Residual) & Risk Treatment |
| **Action Tracker & Remediation Plan** | SLA-Driven Remediation Scheduling & Completion Evidence Tracking |
| **Operational SOPs (`sops/` directory)** | Privacy Operations (DSAR), AI Governance (RAG Testing), & Vendor Risk (TPRM) |

---

# 1. Executive Summary & Dashboard

### Assessment at a Glance
- **Business Context:** Island Shores Artisans & Tours is a fictional 15-employee retail and guided tour business operating in Charlottetown, PEI. To automate customer inquiry response times during peak travel seasons, the business is evaluating the deployment of the **Intercom Fin AI Agent** (a retrieval-augmented generation support system).
- **Assessment Objective:** Evaluate security, AI governance, privacy, and vendor risks associated with integrating Intercom Fin AI into customer support operations.
- **Key Findings:** Intercom demonstrates a mature enterprise security baseline (SOC 2 Type II, ISO 27001, ISO 42001) and zero-retention AI inference contracts with LLM subprocessors (OpenAI/Anthropic). However, **Island Shores faces 4 critical operational/configuration gaps** regarding customer-side chat log retention, cross-border privacy disclosures under PIPEDA, AI hallucination governance, and mandatory AI bot labeling.

```text
========================================================================================
                               EXECUTIVE DASHBOARD
========================================================================================
   [ 04 ]                    [ 05 ]                      [ 03 ]
Primary Risks Identified    Control Frameworks Mapped    Operational SOPs Standardised
----------------------------------------------------------------------------------------
• Cross-Border Transfer    • ISO 27001:2022             • SOP-001: DSAR Playbook
• Chat Retention Gaps      • ISO 42001 (AI Management)  • SOP-002: RAG KB Review
• AI Hallucination         • NIST AI RMF 1.0            • SOP-003: TPRM & Subprocessors
• AI Bot Transparency      • PIPEDA / GDPR              
========================================================================================
```

### Priority Remediation Matrix

| Priority | Risk Finding | Recommended Action | Owner | Target Timeline | Status / Evidence Required |
| :---: | :--- | :--- | :--- | :--- | :--- |
| **01** | **Undisclosed Cross-Border AI Processing** | Update website Privacy Policy to explicitly disclose US-based AI subprocessor data flows under PIPEDA. | Legal / Operations | Prior to System Launch | Updated Privacy Policy published on website. |
| **02** | **Over-Retention of Customer Chat Logs** | Configure automated Intercom inbox retention rules to purge chat logs after 12 months; enforce mandatory 2FA/SSO for all staff. | IT Administrator | During Initial Setup | Intercom retention settings screenshot & Okta/2FA enforcement log. |
| **03** | **AI Hallucination on Booking & Refund Terms** | Restrict Fin KB to vetted FAQs; conduct 10 adversarial edge-case simulation tests in Intercom testing environment. | Customer Support Lead | 2 Weeks Prior to Launch | Simulation test log & signed KB sign-off sheet. |
| **04** | **Mandatory AI Agent Disclosure** | Ensure Intercom's "Show AI Agent label" remains permanently active and greeting message explicitly identifies AI status. | Customer Support Lead | Prior to System Launch | Active Intercom Messenger UI configuration audit. |

---

# 2. Scope, Assessment Methodology & Limitations

### 5-Stage GRC Assessment Methodology

```text
  ┌──────────────┐     ┌──────────────┐     ┌──────────────┐     ┌──────────────┐     ┌──────────────┐
  │  1. IDENTIFY │ ──> │   2. ASSESS  │ ──> │   3. MAP     │ ──> │  4. EVALUATE │ ──> │ 5. REMEDIATE │
  └──────────────┘     └──────────────┘     └──────────────┘     └──────────────┘     └──────────────┘
   • Business Use       • Vendor Security    • ISO 27001          • Inherent Risk      • Action Tracker
   • Data Categories    • AI Controls        • ISO 42001          • Existing Controls  • SOP Protocols
   • Subprocessors      • Config Gaps        • NIST AI RMF        • Residual Risk      • TPRM Oversight
   • Regulations        • Privacy Rules      • PIPEDA / GDPR      • Risk Treatment     • Owner SLAs
```

1. **Identify:** Define business context, data inputs (PII, chat context), subprocessor supply chain (AWS, OpenAI, Anthropic), and legal requirements.
2. **Assess:** Analyze vendor certifications, Trust Center artifacts, Data Processing Agreements (DPAs), and platform settings.
3. **Map:** Align vendor implementation and customer responsibilities against ISO 27001:2022, ISO 42001, NIST AI RMF, and PIPEDA/GDPR principles.
4. **Evaluate:** Calculate inherent risk, evaluate control effectiveness, and determine precise residual risk ratings.
5. **Remediate:** Formulate operational action plans, establish Standard Operating Procedures (SOPs), and set ongoing monitoring cadences.

### Evidence Classification Framework

To ensure professional analytical rigor, evidence utilized in this assessment is categorized into four distinct levels:

*   **Level 1 — Vendor Documentation (Third-Party Claims):** SOC 2 Type II Report, ISO 27001/42001 Certificates, Intercom Security Trust Center, AIUC-1 Certification, Intercom DPA, and Subprocessor Directory.
*   **Level 2 — Independent Assessment Findings:** Gap analysis of active tenant default configurations, data flow tracing across VPC gateways, and control mapping.
*   **Level 3 — Customer Responsibility (Enforcement):** Island Shores workspace security configurations, employee access controls (MFA/SSO), retention policy settings, and Knowledge Base management.
*   **Level 4 — Remediation Artifacts:** Formal SOPs, testing logs, Privacy Policy amendments, and compliance registers.

### Assessment Limitations & Key Assumptions

> **Disclaimer & Scope Limits:** This assessment is a simulated third-party risk and AI governance project produced using publicly available vendor documentation and a fictional business scenario (*Island Shores Artisans & Tours*). It does not constitute a formal legal opinion, regulatory audit, or penetration test.

*   **Assumption 1:** Island Shores is subject to Canadian federal privacy law under PIPEDA and obligations under GDPR for EU tourists.
*   **Assumption 2:** Intercom operates in accordance with its published security documentation, SOC 2 reports, and zero-retention AI subprocessor agreements.
*   **Assumption 3:** Customer-side controls (MFA, RBAC, KB curation) have not been independently audited and require customer verification.

---

# 3. System Architecture, Data-Flow & Shared Responsibility

### Data Processing Pipeline

1. **Ingestion:** Tourist enters contact information (Name, Email, Phone Number) and inquiry text (booking references, tour schedules, sentiment) via the Intercom Web Widget.
2. **Context Assembly:** Intercom fetches relevant customer attributes and approved Knowledge Base (KB) articles from Island Shores' workspace repository.
3. **In-Transit Processing:** Prompts are encrypted via TLS 1.3 and routed to Intercom's Virtual Private Cloud (VPC) gateway. API calls are dispatched to third-party LLM subprocessors (OpenAI / Anthropic).
4. **Third-Party AI Inference:** Subprocessors process text under **Zero Data Retention** contractual terms (no model training, immediate memory purge upon response generation).
5. **Storage at Rest:** Conversation transcripts and customer profile data are stored in AWS databases (`us-east-1` or `eu-west-1` for EU residency) using AES-256 encryption.

### Architecture & Data-Flow Map

```text
                     ISLAND SHORES TOURIST / WEBSITE VISITOR
                                        │
                                        ▼ (HTTPS / TLS 1.3 Encryption)
                           ┌─────────────────────────┐
                           │   Intercom Messenger    │
                           │       (Widget)          │
                           └────────────┬────────────┘
                                        │
                                        ▼
                           ┌─────────────────────────┐
                           │  Intercom VPC Gateway   │
                           │   (Ingestion & Routing) │
                           └────────────┬────────────┘
                                        │
          ┌─────────────────────────────┴─────────────────────────────┐
          ▼                                                           ▼
┌───────────────────────────┐                               ┌───────────────────────────┐
│ Island Shores Internal KB │                               │  Customer Workspace Context│
│ • Tour Schedules & Rates  │                               │  • Tourist PII (Name, Email)│
│ • Refund & Weather Rules  │                               │  • Booking Reference      │
└─────────┬─────────────────┘                               └───────────┬───────────────┘
          │                                                             │
          └─────────────────────────────┬───────────────────────────────┘
                                        │ (RAG Prompt Construction)
                                        ▼
                           ┌─────────────────────────┐
                           │   Intercom Fin AI       │
                           │   Orchestration Engine  │
                           └────────────┬────────────┘
                                        │
          ┌─────────────────────────────┴─────────────────────────────┐
          ▼ (REST API / Zero-Retention)                               ▼ (Encrypted Storage)
┌───────────────────────────┐                               ┌───────────────────────────┐
│ Third-Party LLM Vendors   │                               │ AWS Data Infrastructure   │
│ • OpenAI (US)             │                               │ • Region: us-east-1 / eu  │
│ • Anthropic (US)          │                               │ • Storage: AES-256        │
│ • Google Cloud (US)       │                               │ • Active Chat Retention   │
└───────────────────────────┘                               └───────────────────────────┘
```

### Shared Responsibility Matrix

> **KEY GRC FINDING:** SaaS vendors manage platform infrastructure security, but customers remain fully accountable for access management, data governance, knowledge accuracy, and legal compliance.

| Control Area | Intercom (Vendor) Responsibility | Island Shores (Customer) Responsibility |
| :--- | :--- | :--- |
| **Data Encryption** | Enforce TLS 1.3 in transit and AES-256 at rest across AWS DBs. | Deploy widget strictly on secure HTTPS website domains. |
| **Identity & Access** | Provide SSO, SCIM, 2FA, and granular RBAC platform capabilities. | Enforce mandatory 2FA/SSO and perform quarterly admin access reviews. |
| **AI Inference Privacy** | Enforce zero-retention DPAs prohibiting LLM model training. | Disclose third-party AI processing in Privacy Policy. |
| **Data Retention** | Maintain platform deletion capability upon workspace termination. | Configure automated chat transcript retention and purge rules (e.g., 12 mos). |
| **AI Safety & Accuracy**| Provide RAG architecture, confidence thresholds & simulation tools. | Maintain accurate, curated Knowledge Base articles and test edge cases. |
| **Subprocessor Oversight**| Publish controlled subprocessor directories and send 20-day notices. | Subscribe to vendor change alerts and evaluate new AI subprocessor DPAs. |

---

# 4. Control Assessment Matrix

The following matrix maps Intercom's published security and AI controls alongside Island Shores' required operational safeguards against **ISO 27001:2022**, **ISO 42001 (AI Management)**, and the **NIST AI Risk Management Framework (NIST AI RMF 1.0)**.

| Framework Ref | Control Objective | Vendor Implementation | Evidence Source | Status | Customer Enforcement Requirement |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **NIST Govern 1.1**<br>ISO 42001 A.5.1 | Establish AI governance, policies, and accountability structures. | Intercom maintains formal AI governance validated via ISO 42001 and AIUC-1 certifications. | ISO 42001 Cert & Trust Center | **Addressed** | Assign internal AI governance owner (Customer Support Lead). |
| **NIST Map 3.1**<br>ISO 27001 A.5.21 | Manage security across the ICT supply chain and AI subprocessors. | Enforces strict DPAs with OpenAI/Anthropic featuring zero data retention and no model training. | Intercom Subprocessor List & DPA | **Addressed** | Subscribe to subprocessor change alerts and review 20-day change notices. |
| **NIST Measure 2.6**<br>ISO 42001 A.8.8 | Manage AI safety, hallucinations, and output reliability. | Uses RAG grounded strictly in customer KB articles; triggers human escalation when confidence is low. | Intercom Fin Product Documentation | **Addressed** | Audit KB quarterly and conduct adversarial testing before publishing KB updates. |
| **NIST Manage 2.1**<br>ISO 27001 A.8.24 | Protect customer data via strong cryptographic controls. | Enforces AES-256 encryption at rest and TLS 1.3 in transit; supports SSO and 2FA. | SOC 2 Type II Report (CC6.1, CC6.7) | **Addressed** | Enforce 2FA/SSO across all staff accounts accessing the Intercom workspace. |
| **NIST Manage 2.3**<br>ISO 27001 A.8.10 | Enforce information retention and data deletion practices. | Deletes workspace data within 30 days of contract termination. | Intercom Privacy Policy | **Partially Addressed** | **GAP:** Configure active inbox retention rules (e.g., 12-month auto-deletion). |
| **PIPEDA Principle 4.3**<br>GDPR Art. 13 | Provide transparency regarding automated decision-making and AI use. | Provides configurable "Show AI Agent label" in Messenger UI. | Intercom Admin Console Settings | **Partially Addressed** | **GAP:** Keep AI label active and mandate explicit AI identification in greeting. |

---

# 5. Privacy & Regulatory Assessment (PIPEDA & GDPR)

### Regulatory Compliance Matrix

| Requirement | Applicability | Current State | Identified Gap | Recommended Remediation |
| :--- | :--- | :--- | :--- | :--- |
| **Transparency & Consent** *(PIPEDA Princ. 4.3 / GDPR Art. 13)* | **High** (Mandatory for tourist inquiry chat) | Intercom offers default AI bot labeling. | Website Privacy Policy does not disclose automated AI processing or US transfers. | Amend Privacy Policy to explicitly outline third-party AI processing and bot interaction. |
| **Cross-Border Transfers** *(PIPEDA Princ. 4.1 / GDPR Ch. V)* | **High** (AWS Dublin residency; US LLMs) | Data processing occurs via US OpenAI/Anthropic APIs. | Potential compliance gap if cross-border transfer is unannounced. | Add cross-border processing notice to Privacy Policy and confirm vendor DPA SCCs. |
| **Data Minimization & Retention** *(PIPEDA Princ. 4.5 / GDPR Art. 5(1)(e))* | **High** (PII collected during bookings) | Zero retention at LLM layer; indefinite chat retention in Intercom inbox. | Active tenant chat logs stored indefinitely without automated purge. | Implement automated 12-month chat log deletion rule in Intercom settings. |
| **Data Subject Access Requests** *(PIPEDA Princ. 4.9 / GDPR Art. 15-17)* | **High** (Right to access/delete tourist PII) | Intercom provides manual "Export" and "Delete User" buttons. | No formal staff procedure to verify identities or meet 30-day SLA. | Implement **SOP-001 (DSAR Playbook)** with identity verification and 30-day logging. |

### Key Regulatory Analysis

1. **Cross-Border Transfer Dynamics (PIPEDA):** While Island Shores can select EU AWS data storage (Dublin), AI inference requests pass through US-based LLM APIs (OpenAI/Anthropic). Under PIPEDA, organization accountability requires informing individuals that their personal information may be processed in foreign jurisdictions and subject to foreign access laws.
2. **Automated AI Processing Transparency:** Both Canadian OPC guidelines and EU GDPR rules prohibit misrepresenting AI agents as human staff. Island Shores must ensure Intercom's AI agent visual badge is permanently enabled.

---

# 6. Risk Assessment & Risk Register

### Risk Scoring Methodology

Inherent and Residual Risks are calculated using a $5 \times 5$ Risk Matrix:

$$\text{Inherent Risk} = \text{Likelihood (1--5)} \times \text{Impact (1--5)}$$

*   **Likelihood:** 1 (Rare), 2 (Unlikely), 3 (Possible), 4 (Likely), 5 (Almost Certain)
*   **Impact:** 1 (Insignificant), 2 (Minor), 3 (Moderate), 4 (Major), 5 (Catastrophic)
*   **Risk Bands:** Low (1–6) | Medium (8–12) | High (15–25)

```text
                  LIKELIHOOD
        1       2       3       4       5
     ┌───────┬───────┬───────┬───────┬───────┐
   5 │   5   │  10   │  15   │  20   │  25   │
I    ├───────┼───────┼───────┼───────┼───────┤
M  4 │   4   │   8   │  12   │ [R02] │  20   │
P    ├───────┼───────┼───────┼───────┼───────┤
A  3 │   3   │   6   │  9    │ [R01] │  15   │
C    ├───────┼───────┼───────┼───────┼───────┤
T  2 │   2   │   4   │   6   │   8   │  10   │
     ├───────┼───────┼───────┼───────┼───────┤
   1 │   1   │   2   │   3   │   4   │   5   │
     └───────┴───────┴───────┴───────┴───────┘
```

### Comprehensive Risk Register

| Risk ID | Risk Scenario & Finding | L | I | Inherent Risk | Vendor Controls | Customer Safeguards & Treatment | Residual Risk |
| :--- | :--- | :---: | :---: | :---: | :--- | :--- | :---: |
| **R-01** | **AI Hallucination:** Fin provides incorrect pricing, refund terms, or tour schedules, causing financial loss or customer disputes. | 4 | 3 | **High (12)** | RAG architecture restricted to KB; confidence thresholds trigger human escalation. | **Mitigate:** Curate KB strictly; mandate SOP-002 adversarial testing before publishing updates. | **Low (4)** |
| **R-02** | **Undisclosed Cross-Border Data Processing:** Tourist PII is processed by US LLMs without disclosure, leading to PIPEDA complaints. | 3 | 4 | **High (12)** | Subprocessor DPAs with Standard Contractual Clauses (SCCs). | **Mitigate:** Update website Privacy Policy to disclose US AI processing prior to launch. | **Low (3)** |
| **R-03** | **PII Exposure via LLM Model Training:** Tourist PII entered into chat is ingested into public LLM training sets. | 2 | 4 | **Medium (8)** | Zero-retention DPAs; contractual ban on model training. | **Accept & Monitor:** Conduct annual TPRM reviews (SOP-003) to ensure zero-retention contract terms remain active. | **Low (2)** |
| **R-04** | **Unauthorized Workspace Access:** Compromised staff credentials expose customer chat database and tourist PII. | 3 | 4 | **High (12)** | Intercom platform support for 2FA, SSO, and granular RBAC. | **Mitigate:** Enforce mandatory 2FA/SSO on all staff accounts. *Residual rating contingent on 2FA enforcement.* | **Low (3)\*** |

---

# 7. Action Tracker & Remediation Roadmap

| Task ID | Remediation Action | Assigned Owner | SLA / Target Date | Required Completion Evidence | Review Cadence |
| :---: | :--- | :--- | :--- | :--- | :--- |
| **ACT-01** | Revise Privacy Policy with AI & Cross-Border disclosures. | Legal / Operations | 1 Week Pre-Launch | Live website URL & legal sign-off document. | Annual |
| **ACT-02** | Enforce 12-month chat auto-deletion rule in Intercom. | IT Administrator | Initial Setup | Admin Console settings export/screenshot. | Semi-Annual |
| **ACT-03** | Mandate 2FA/SSO enforcement for all Intercom users. | IT Administrator | Immediate | Okta / Intercom authentication policy log. | Quarterly |
| **ACT-04** | Complete initial adversarial simulation testing on KB. | Customer Support Lead | 2 Weeks Pre-Launch | Completed SOP-002 Test Log with 10 test scenarios. | Quarterly |
| **ACT-05** | Activate official Subprocessor Notification subscription. | IT Administrator | Immediate | Intercom subprocessor notification confirmation email. | Ongoing |

---

# 8. Operational Standard Operating Procedures (SOPs)

The detailed, standalone operational procedures are located in the [`sops/`](./sops/) folder of this repository:

1. [**SOP-001: Data Subject Access Request (DSAR) Playbook**](./sops/SOP-001-DSAR-Playbook.md)  
   - **Focus:** Step-by-step workflow for intake, identity verification, user profile export/deletion in Intercom, and 30-day compliance logging under PIPEDA & GDPR.
2. [**SOP-002: AI Knowledge Base (RAG) Governance Procedure**](./sops/SOP-002-RAG-Governance.md)  
   - **Focus:** Lifecycle management of Knowledge Base content, quarterly/pre-peak season auditing, pruning legacy tour rules, and executing 10 adversarial simulation tests in Intercom's sandbox.
3. [**SOP-003: Third-Party Risk Management (TPRM) Procedure**](./sops/SOP-003-TPRM-Monitoring.md)  
   - **Focus:** Continuous vendor oversight, automated subprocessor tracking, 20-day DPA evaluation windows for zero-retention compliance, and annual SOC 2 / ISO 42001 Trust reviews.

---

# 9. How to Use This Case Study

This repository serves as a practical demonstration of GRC engineering and risk consulting capabilities. 

* **Recruiters & Hiring Managers:** Review the [Priority Remediation Matrix](#priority-remediation-matrix), [Shared Responsibility Matrix](#shared-responsibility-matrix), and [Control Assessment Matrix](#4-control-assessment-matrix) above for a direct overview of assessment rigor.
* **Operational Execution:** Examine the standalone playbooks in the [`sops/`](./sops/) directory for ready-to-deploy operational workflows.
* **Offline Review:** Download [`grc-intercom-project.docx`](./grc-intercom-project.docx) for the fully formatted executive deliverable.
