# SOP-002: AI Knowledge Base (RAG) Governance Procedure

| Metadata Field | Document Details |
| :--- | :--- |
| **Document ID** | SOP-002 |
| **Effective Date** | October 1, 2026 |
| **Owner** | Customer Support Lead |
| **Approver** | Operations Manager |
| **Review Cadence** | **Quarterly** (Mandatory Pre-Peak Season Review in April/May) |
| **Applicable System** | Intercom Fin Knowledge Base & Testing Sandbox |

---

## 1. Purpose & Scope
To govern the lifecycle of Knowledge Base (KB) articles feeding Intercom Fin AI (Retrieval-Augmented Generation pipeline), preventing AI hallucinations, pricing inaccuracies, outdated tour policies, and brand misrepresentation.

---

## 2. Procedure Workflow

```text
┌──────────────────┐     ┌──────────────────┐     ┌──────────────────┐     ┌──────────────────┐
│  1. AUDIT &      │ ──> │  2. PRUNE &      │ ──> │  3. SIMULATION   │ ──> │  4. APPROVE &    │
│     SCHEDULE     │     │     REVISE       │     │     TESTING      │     │     LOG          │
└──────────────────┘     └──────────────────┘     └──────────────────┘     └──────────────────┘
 • Quarterly Review       • Unambiguous Text       • 10 Edge Cases          • Version Control
 • Pre-Season Audit       • Archive Old Tours      • Intercom Sandbox       • Update KB Log
```

### **Step 1: Review Scheduling**
* Conduct formal audits quarterly. Mandate a comprehensive audit every **April/May** prior to peak tourist season to update tour schedules, pricing, and cancellation rules.

### **Step 2: Article Pruning & Precision Drafting**
* Review all active KB articles. Replace ambiguous statements (e.g., *"We usually refund cancellations"*) with strict rules (e.g., *"Cancellations made 48+ hours prior to tour departure receive a 100% refund"*).
* **Archive Outdated Content:** Fully archive retired tour descriptions rather than unlisting them to ensure LLM retrieval cannot index legacy policies.

### **Step 3: Adversarial Simulation Testing**
* Import draft articles into Intercom Fin's testing sandbox.
* Execute **10 adversarial prompts** targeting edge cases (e.g., severe weather cancellations, flight delays, partial party refunds, off-season booking attempts).
* Verify that Fin grounds answers solely in KB text and correctly triggers human escalation when confidence is low.

### **Step 4: Approval & Version Control**
* Obtain Customer Support Lead approval, publish articles to live workspace, and record version changes in the Knowledge Base Governance Register.

---

## 3. Quality Standards & Hallucination Prevention
* **Grounding Threshold:** Fin AI must strictly answer based on provided Knowledge Base articles.
* **Escalation Trigger:** Any prompt falling below confidence thresholds must immediately route to human customer support agents with full conversation context attached.
