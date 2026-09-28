# SOP-003: Third-Party Risk Management (TPRM) Procedure

| Metadata Field | Document Details |
| :--- | :--- |
| **Document ID** | SOP-003 |
| **Effective Date** | October 1, 2026 |
| **Owner** | IT Administrator |
| **Approver** | Operations Manager |
| **Review Cadence** | **Annual Trust Review** + Ongoing Subprocessor Change Monitoring |
| **Applicable System** | Intercom Trust Center, Subprocessor Directory & Vendor DPAs |

---

## 1. Purpose & Scope
To monitor cybersecurity, privacy, and vendor supply chain risks associated with Intercom and its subprocessor ecosystem (including OpenAI, Anthropic, and AWS).

---

## 2. Procedure Workflow

```text
┌──────────────────┐     ┌──────────────────┐     ┌──────────────────┐     ┌──────────────────┐
│  1. SUBPROCESSOR │ ──> │  2. 20-DAY DPA   │ ──> │  3. ANNUAL TRUST │ ──> │  4. RENEWAL      │
│     SUBSCRIPTION │     │     EVALUATION   │     │     AUDIT        │     │     ALIGNMENT    │
└──────────────────┘     └──────────────────┘     └──────────────────┘     └──────────────────┘
 • Subprocessor Alert     • Check Zero-Retention  • SOC 2 / ISO 42001      • OPC/PIPEDA Review
 • RSS / Email Register   • Option to Object      • CUEC Verification      • Contract Terms
```

### **Step 1: Subprocessor Tracking Subscription**
* Subscribe IT Administrator to Intercom's official Subprocessor Notification directory.

### **Step 2: Managing 20-Day Subprocessor Change Notices**
* Upon receipt of a vendor change notice, review new subprocessor details within the contractually mandated **20-day window**.
* Verify that any new AI subprocessor commits to zero data retention for model training and enforces encryption in transit. If non-compliant, formally object via DPA mechanisms or disable Fin AI.

### **Step 3: Annual Trust Artifact Review (Every January)**
* Download latest SOC 2 Type II report, ISO 27001, and ISO 42001 certificates from Intercom's Trust Center.
* Verify SOC 2 report opinion (ensure no qualified opinions on core security or privacy controls).
* Audit **Complementary User Entity Controls (CUECs)** to confirm Island Shores continues meeting customer obligations (e.g., 2FA/SSO enforcement, role-based access control).

### **Step 4: Renewal Alignment & Regulatory Review**
* 60 days prior to contract renewal, review OPC guidance updates and confirm Intercom DPA terms remain compliant with federal privacy standards under PIPEDA.

---

## 3. Vendor Review Thresholds
* **Critical Subprocessors:** OpenAI, Anthropic, AWS (must maintain zero-retention API policies and ISO 27001 / SOC 2 Type II compliance).
* **Remediation Action:** If a subprocessor loses certification or modifies zero-retention commitments, escalate to Operations Manager within 24 hours.
