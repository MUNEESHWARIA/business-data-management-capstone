# Insurance Claims Operations Analytics — Right View Investigators

> **Turning operational data into strategic decisions for a motor insurance investigation firm.**

---

## Business Context

**Right View Investigators (RVI)** is a Madurai-based private investigation firm serving major Indian insurance companies — including Chola, Magma, Shriram, and Liberty Insurance — across third-party motor claims, bodily injury cases, and own-damage investigations.

Despite handling **1,000+ active cases**, the firm operated with manual Excel tracking, no revenue visibility, and zero analytical infrastructure. This project built a full-scale data analytics solution directly from their operational records — identifying where money was stuck, where cases were stalling, and what the business needed to do next.

---

## The Business Problem

Three critical gaps were costing RVI time and money:

- **Operational blind spots** — No structured tracking of case turnaround times or workload distribution across investigators
- **Revenue leakage** — ₹3.29M in unrealized income with no automated follow-up or monitoring system
- **No data-driven strategy** — Decisions were being made on intuition, not evidence

---

## Dataset Overview

| Attribute | Detail |
|---|---|
| **Source** | Live operational records — `Combine RTI and Case Status Trial` |
| **Period Covered** | January – June 2025 |
| **Total Records** | 1,079 unique investigation cases |
| **Fields** | 26 variables across operational, financial, investigative & admin domains |
| **Collection Method** | Direct extraction from RVI's internal Excel tracking system |

**Key field categories:**
- Operational: Claim No., Status, Turnaround Time (TAT)
- Investigation: Type, Police Station, RTI Date
- Financial: Claim Amount, Fee Receipt, Payment Status
- Administrative: Reporter, Mail Status, Dispatch Date

---

## Data Preparation

Before analysis, the dataset underwent structured cleaning:

- Removed **3 duplicate records** (1,082 → 1,079 clean records)
- Standardized all date formats to `DD/MM/YYYY`
- Imputed **45% missing Submitted Dates** using Dispatch Date as a reliable proxy
- Unified inconsistent column naming and corrected data type mismatches
- Validated all financial fields for outliers using Z-score thresholds

---

## Methodology

**Statistical techniques applied:**

- **Descriptive Statistics** — Distribution profiling of TAT, claim amounts, and case volumes
- **Chi-Square Test** — Tested independence between claim type and resolution status (χ² = 30.62, p < 0.001)
- **Z-Score Analysis** — Flagged 12 extreme TAT outliers and 5 anomalous fee cases
- **Correlation Analysis** — Confirmed no pricing dependency on TAT (R² = 0.005)
- **Revenue Gap Analysis** — Quantified total unrealized income by status category

**Tools used:**

| Purpose | Tools |
|---|---|
| Data Cleaning & Structuring | Microsoft Excel, Google Sheets |
| Statistical Analysis | Python (Pandas, NumPy, SciPy) |
| Visualization | Excel Charts, Pivot Tables |
| Reporting & Presentation | PowerPoint, PDF |

---

## Key Insights

### ⏱ Turnaround Time is High and Inconsistent
- Average TAT: **87.5 days** | Median: **77 days** | Mode: **18 days**
- Standard deviation of **67.7 days** signals severe inconsistency in case handling
- Maximum TAT recorded: **589 days** — clear evidence of cases falling through the cracks
- Right-skewed distribution confirms a minority of cases are dragging overall averages up

### 💰 Revenue is Tied Up and Untracked
- **₹2.14M** locked in submitted-but-unpaid cases
- **₹1.15M** stuck in pending cases with no automated escalation
- Total revenue gap: **₹3.29M** — unmonitored and unrecovered

### 📋 Case Backlog is Concentrated in Third-Party Claims
- **688 of 1,079 cases** are Third-Party (TP) claims
- TP cases have a **37.6% pending rate** vs. 25.6% for Non-TP cases
- Only **62% of total cases** have been submitted; **33% remain pending**

### 🏢 Client Concentration Poses a Risk
- Top two clients — **Chola (18%) and Magma (17%)** — account for 35% of all cases
- No structured SLA tracking exists for high-value client relationships
- Heavy dependency on two clients creates revenue vulnerability

### 📊 Pricing is Standardized but Underoptimized
- Most claims fall in the **₹1,500–₹5,500** band (Average: ₹3,192 | Median: ₹3,600)
- No correlation between case complexity (TAT) and fee charged (R² = 0.005)
- One-size-fits-all pricing leaves money on the table for complex, high-effort cases

---

## Business Recommendations

### 1. Implement Case-Type SLAs
Define turnaround benchmarks by case type (TP vs. Non-TP, bodily injury vs. OD). Automate alerts at 60-day and 90-day thresholds to prevent cases from aging silently.

### 2. Build a Revenue Recovery Pipeline
Flag and escalate all pending fee cases weekly. Assign ownership for follow-up on the ₹1.15M currently sitting untracked. Target: **₹200,000+ recovered within the first quarter of implementation.**

### 3. Introduce Tiered Pricing
Charge a complexity premium for cases that exceed median TAT by more than one standard deviation. This aligns revenue with actual investigative effort and improves margin on high-effort cases.

### 4. Reduce Client Concentration Risk
Actively develop 3–4 new insurer relationships to reduce Chola + Magma dependency below 25%. Create dedicated account management for top clients with formal SLA compliance reporting.

### 5. Replace Manual Tracking with a Structured Dashboard
Move from Excel to a real-time operations dashboard tracking TAT, case status, client distribution, and revenue by week. This alone can reduce reporting time by an estimated **5–8 hours per week.**

---

## Expected Impact

| Outcome | Target |
|---|---|
| Case backlog reduction | 20% within 6 months |
| SLA compliance for key clients | 90%+ |
| Revenue recovered from pending cases | ₹200,000+ |
| Data accuracy improvement | 90%+ |
| Reporting time saved per week | 5–8 hours |

---

## Project Files

| File | Description |
|---|---|
| `Combine RTI and Case Status Trial_Midterm.xlsx` | Primary operational dataset |
| `BDM-Proposal.pdf` | Project scope and analytical plan |
| `BDM-Midterm Report.pdf` | Interim analysis and data preparation findings |
| `BDM-Final Report.pdf` | Complete analysis, results, and recommendations |
| `Insurance_Claims_Analytics_Presentation.pptx` | Executive summary deck |

---

## Tech Stack

`Python` · `Pandas` · `NumPy` · `SciPy` · `Microsoft Excel` · `Google Sheets` · `PowerPoint`

---

## About

**Analyst:** Muneeshwari N  
**Domain:** Insurance Operations & Business Analytics  
**Organization studied:** Right View Investigators, Madurai, Tamil Nadu  
**Data period:** January – June 2025
