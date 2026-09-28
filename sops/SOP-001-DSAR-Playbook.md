# SOP-001: Data Subject Access Request (DSAR) Playbook

| Metadata Field | Document Details |
| :--- | :--- |
| **Document ID** | SOP-001 |
| **Effective Date** | October 1, 2026 |
| **Owner** | Customer Support Lead |
| **Approver** | Operations Manager |
| **SLA Requirement** | **30 Calendar Days** (PIPEDA Principle 4.9 / GDPR Art. 15–17) |
| **Applicable System** | Intercom Admin Console & Workspace Contacts |

---

## 1. Purpose & Scope
This Standard Operating Procedure (SOP) defines the operational workflow for receiving, verifying, executing, and logging Data Subject Access Requests (DSARs) submitted by customers requesting data access or permanent erasure regarding personal data processed by Intercom Fin AI Agent.

---

## 2. Procedure Workflow

```text
┌──────────────────┐     ┌──────────────────┐     ┌──────────────────┐     ┌──────────────────┐
│  1. INTAKE &     │ ──> │  2. INTERCOM     │ ──> │  3. EXECUTE      │ ──> │  4. LOG &        │
│     VERIFY       │     │     SEARCH       │     │     ACCESS/ERASE │     │     CONFIRM      │
└──────────────────┘     └──────────────────┘     └──────────────────┘     └──────────────────┘
 • Dedicated Inbox        • Search Contact         • Option A: Export       • Update Tracker
 • Confirm Identity       • Check Email Match      • Option B: Delete       • Notify Customer
```

### **Step 1: Intake & Identity Verification**
* Direct all privacy inquiries to `privacy@islandshores.ca`.
* **Mandatory Verification:** Before releasing or deleting data, verify requester identity against an email confirmation link or a valid booking reference number. *Never export records to an unverified email address.*

### **Step 2: Data Search & Retrieval**
* Log into the Intercom Admin Console $\rightarrow$ Navigate to **Contacts**.
* Search for the verified customer email address.

### **Step 3: Execution (Access vs. Erasure)**
* **Option A (Right to Access):** Open user profile $\rightarrow$ Select **Export User Data**. Review generated file for third-party PII (e.g., credit card numbers mentioned in chat) and redact as necessary. Transmit securely to customer within the 30-day window.
* **Option B (Right to Erasure):** Open user profile $\rightarrow$ Select **Delete User**. Confirm permanent removal of customer profile and associated chat transcripts across Intercom databases.

### **Step 4: Logging & Closure**
* Record request type, date received, verification status, completion date, and admin ID in the secure Privacy Compliance Log. Transmit written confirmation to requester within 30 days.

---

## 3. Compliance Standard & SLA Control
* **Statutory SLA:** Requests must be completed within 30 calendar days under PIPEDA and GDPR.
* **Exceptions:** If identity verification fails or an extension is legally permitted, log the justification in the Privacy Compliance Log and notify the applicant prior to Day 30.
