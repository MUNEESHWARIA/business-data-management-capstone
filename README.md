# business-data-management-capstone
"Comprehensive data analysis project applying statistical methods to real-world business scenarios"
📊 Business Analytics Solution for Investigating Third-Party Motor Insurance Claims

A Case Study of Right View Investigators, Madurai

👩‍💼 Author: Muneeshwari N

Roll Number: 24ds3000101
Program: IITM Online BS Degree in Data Science
Institution: Indian Institute of Technology, Madras

🧭 Project Overview

This project presents a data-driven business analytics solution designed to improve operational efficiency, financial tracking, and decision-making at Right View Investigators, a private investigation firm specializing in third-party motor insurance claim investigations.

By applying advanced statistical and analytical techniques, the study identifies key performance gaps, quantifies inefficiencies, and recommends actionable strategies for optimization.

🏢 About the Organization

Right View Investigators (RVI), established in 2017 and based in Madurai, Tamil Nadu, provides investigative services for insurance companies across India.
Their primary focus areas include:

Third-Party Bodily Injury and Fatal Claims

Own Damage (OD) Claims

Motor Accident Reconstructions

Connected Investigations

Key clients include Chola, Magma, Shriram, and Liberty Insurance, making RVI a trusted partner for major insurers.

⚙️ Problem Statement

RVI faced three major operational challenges:

Manual Tracking Inefficiencies – Excel-based tracking of 1,000+ cases led to inconsistent data and delayed processing.

Revenue Monitoring Gaps – ₹1.15 million in pending payments were untracked and unmonitored.

Lack of Analytical Insights – No system for fraud detection, trend analysis, or performance forecasting.

📂 Dataset & Metadata

Data Source: Real operational Excel dataset — “Combine RTI and Case Status Trial”
Duration: January to June 2025
Records: 1,079 unique cases
Variables: 26 operational fields grouped into:

Operational Fields (Claim No., Status, TAT)

Investigation Fields (Type, Police Station, RTI Date)

Financial Fields (Amount, Fee Receipt)

Administrative Fields (Reporter, Mail Status)

Key Statistics:

Metric	Value
Average Turnaround Time	87.5 days
Average Claim Amount	₹3,192
TP (Third-Party) Cases	688
Submitted Status	62% of total cases
🧹 Data Cleaning & Preparation

A rigorous cleaning process was applied:

Removed duplicates (1082 → 1079 records)

Standardized date formats (DD/MM/YYYY)

Imputed 45% missing Submitted Dates using Dispatch Dates

Unified column naming and ensured correct data types

📊 Analytical Methods

The following analytical techniques were applied:

Descriptive Statistics: Mean, Median, Mode, Standard Deviation

Chi-Square Test: Relationship between claim type and status (χ² = 30.62, p < 0.001)

Z-Score Analysis: Identified 12 extreme TAT outliers and 5 unusual fee cases

Correlation Analysis: R² = 0.005 → no link between fee and TAT

Revenue Gap Analysis: Quantified ₹3.29M in unrealized income

Tools Used:

Google Sheets, Microsoft Excel, Python (Pandas, NumPy)

📈 Key Results & Findings
🔹 Turnaround Time (TAT)

Mean: 87.5 days, Median: 77 days, Mode: 18 days

Right-skewed distribution → few extreme delays (max: 589 days)

High variability (SD = 67.7 days) → inconsistent case processing

🔹 Claim Amount

Most claims between ₹1,500 – ₹5,500

Average: ₹3,192 | Median: ₹3,600 | Mode: ₹1,800

No correlation between TAT and fees → standardized pricing

🔹 Client Analysis

Top Clients: Chola (18%), Magma (17%)

Combined share: 35% of total cases

Dependency risk identified → recommend client diversification

🔹 Case Status
Status	Count	Percentage
Submitted	670	62%
Pending	356	33%
Completed	43	4%
Withdrawn	7	0.6%

→ TP cases had 37.6% pending rate vs 25.6% for Non-TP cases.

🔹 Financial Insights

₹2.14M tied in submitted cases

₹1.15M in pending cases

Total ₹3.29M of unrealized revenue

💡 Strategic Recommendations
Focus Area	Recommendations	Expected Impact
Operational Efficiency	Implement case-type SLAs, automate alerts, resource balancing	20% backlog reduction
Client Management	Dedicated managers for top clients, SLA compliance tracking	90%+ SLA compliance
Financial Optimization	Tiered pricing for complex cases, revenue follow-up automation	₹200,000 recovery
Data Quality & Reporting	Standardize fields, dropdown data entry, dashboards	90%+ data accuracy
🚀 Expected Business Impact

✅ 20% reduction in backlog
✅ 90% SLA compliance for key clients
✅ ₹200,000 recovered revenue
✅ 90%+ data accuracy and consistency
✅ Real-time tracking and improved decision-making

🧠 Key Insights

Small firms can achieve enterprise-grade efficiency through analytics.

Data quality and structure form the foundation for meaningful analysis.

Statistical testing transforms anecdotal assumptions into measurable insights.

Analytical frameworks are scalable and generalizable to other investigation firms.

🧩 Tools & Technologies
Category	Tools
Data Cleaning	Google Sheets, Excel
Analysis	Python (Pandas, NumPy, SciPy)
Visualization	Excel Charts, Pivot Tables
Reporting	PowerPoint, PDF
Statistical Tests	Chi-Square, Correlation, Z-Score
🔭 Future Scope

Predictive modeling for case duration and fraud detection

Automated dashboards for live SLA and revenue tracking

Integration with a FastAPI backend for data management

Expansion to multi-branch analysis across different cities

🏁 Conclusion

This project demonstrates how data analytics can transform investigative operations in the insurance sector. By identifying inefficiencies, quantifying delays, and recommending strategic improvements, this study provides Right View Investigators with a clear roadmap for achieving sustainable growth and operational excellence.

🙏 Acknowledgement

Special thanks to Right View Investigators, Madurai, for providing access to real operational data, and to the IITM Data Science faculty for their valuable guidance and evaluation framework.
