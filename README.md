# Loan Issuance Automation in LOS System
**Business Analysis | Process Optimization | BPMN | UML | Automation Logic**

---

## 🎯 Goal
Optimize the loan issuance process and **automate second and subsequent loan disbursements**, provided that:
- the first loan’s issuance date is **within the last 12 months**, and  
- the first loan’s checklist status was **not RED**.

---

## 🚩 Problem (Before Automation)
In the AS-IS process:
- **100% of repeat loans** were routed to **manual review** by Credit Risk and Credit Administration.
- Operators manually checked: documents, collateral, tax arrears, scoring, bureau, restrictions.
- SLA violations and bottlenecks were frequent.
- The process was slow, error-prone, and not scalable.

---

## ⭐ Result (After Automation)
- Manual review for repeat loans dropped from **100% → 20–30%**  
- Processing time: **30–60 minutes → under 1 minute**  
- Manual load on Credit Administration decreased dramatically  
- Customer experience improved (near-instant disbursement)  
- LOS system now routes cases automatically using checklist evaluation logic  

---

## 📌 AS-IS Process (Before)
![AS-IS Diagram](./AS-IS.png)

---

## 📌 TO-BE Process (After Automation)
Automation introduced:
- Checklist auto-reading
- Decision Engine routing (auto vs manual)
- Exception handling only for RED status or >12 months

![TO-BE Diagram](./TO-BE.png)

---

## 📌 UML Sequence Diagram – LOS Internal Logic
Checklist Evaluation & Routing Logic  
(How LOS backend determines whether to auto-disburse or route to manual review)

![UML Sequence](./UML.png)

---

