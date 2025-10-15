💰 Bank Loan Report Summary – Power BI Dashboard

🏦 Project Overview
Bank Loan Report Summary is an interactive Power BI dashboard designed to analyze and monitor loan portfolio performance for banks, financial institutions, and microfinance organizations.
It provides a centralized, data-driven view of loan disbursement, repayment trends, and credit risk exposure — empowering management to make smarter, faster lending decisions with real-time insights.

🔑 Key Features

📊 1. Interactive Dashboards

Three comprehensive report views:
•	Summary – Portfolio KPIs and key metrics
•	Overview – Visual analysis by borrower segments and loan types
•	Details – Transaction-level insights for granular drill-down

📈 2. Performance Metrics
<pre> ```
Track critical KPIs with Month-to-Date (MTD) and Month-over-Month (MOM) comparisons:
•	Total Loan Applications
•	Funded Amount
•	Amount Received
•	Average Interest Rate
•	Average Debt-to-Income (DTI) Ratio
 </pre>
💡 3. Loan Segmentation & Risk Analysis
<pre> ```
•	Categorizes Good vs. Bad Loans
•	Visualizes Credit Risk Heatmaps to identify high-risk borrowers
•	Displays loan status breakdown — Fully Paid, Current, Charged Off
 </pre>
🧍 4. Demographic & Categorical Insights
Analyze loans by:
<pre> ```
•	Loan Purpose (debt consolidation, credit card, home improvement, etc.)
•	Home Ownership
•	Employee Length
•	Term Duration (36 vs. 60 months)
•	State or Region
``` </pre>
🔍 5. Drill-Down Functionality

Access detailed insights — including loan ID, grade, sub-grade, funded amount, interest rate, and installment details.


🧩 Problem Statement

Financial institutions handle large volumes of loan data daily — often spread across multiple systems and file formats.
This makes it difficult to monitor performance, identify risks, and maintain data accuracy.
Common challenges include:
<pre> ```
•	❌ High loan default rates due to limited visibility into borrower risk
•	🕒 Time-consuming manual reporting and tracking
•	📉 Lack of real-time portfolio insights
•	📂 Scattered, unstandardized data sources
•	⚠️ Missed early warning signs for bad loans
``` </pre>

🎯 How This Project Helps & Why It’s Useful

The Bank Loan Report Dashboard transforms scattered loan data into interactive, real-time insights — empowering financial institutions to enhance portfolio quality, reduce risk, and improve operational efficiency.


✅ What It Solves
<pre> ```
•	Centralizes Data: Consolidates loan disbursement, repayment, and borrower data in one place
•	Automates KPI Tracking: Calculates and visualizes MTD/MOM metrics instantly
•	Identifies Risk Early: Detects high-risk borrowers and charged-off loans for proactive management
•	Improves Decision-Making: Enables dynamic filtering by state, loan purpose, borrower type, and term
•	Enhances Transparency: Provides real-time portfolio visibility for management and regulatory teams
``` </pre>

💡 Why It’s Valuable
<pre> ```
•	Data-Driven Decisions: Enables smarter, faster lending choices
•	Credit Risk Management: Reduces default exposure through better insights
•	Operational Efficiency: Eliminates manual report preparation with automated dashboards
•	Strategic Planning: Highlights lending trends across states, demographics, and loan purposes
•	Regulatory Compliance: Ensures auditable, transparent reporting
✅ Faster risk detection
✅ Smarter lending decisions
✅ Lower default rates
✅ Improved reporting transparency
``` </pre>

🏗️ Technical Architecture Overview

🔄 Data Flow Diagram

<pre> ```
 📂 Data Sources
 ├── Loan Disbursement Records (CSV / Excel / SQL)
 ├── Repayment History
 └── Customer Profiles
         │
         ▼
🧮 Data Extraction Layer
 ├── Power Query / SQL Scripts
 └── Data Quality Checks
         │
         ▼
📂 Data Transformation
 ├── Cleaning, Merging, Relationships & DAX Measures
 ├── KPIs & Calculated Fields, Data Modeling
         │
         ▼
🧮 Data Model Layer (Star Schema in Power BI)
 ├── Fact: Loan Transactions
 └── Dimensions: Borrower, Purpose, State, Term, etc.
         │
         ▼
💡 Visualization Layer (Power BI Dashboard)
 ├── Summary View (Portfolio KPIs)
 ├── Overview View (Loan Type / Purpose)
 └── Details View (Customer-Level Insights)
         │
         ▼
📊 Publishing & Access Layer
 ├── Power BI Service / Workspace
 └── Role-Based Access Control (RBAC )
``` </pre>

🔧 Architecture Components Explained
1. Data Sources
   <pre> ```
•	Loan Application Data: Loan ID, amount, grade, purpose, term, interest rate, DTI, and borrower details
•	Status Data: Loan repayment status — Fully Paid, Current, or Charged Off
•	Demographic Data: Purpose, state, employee length, home ownership
•	Formats: Excel, CSV, or SQL database
`` </pre>
3. Data Extraction Layer
•	Managed using Power Query or SQL scripts
•	Connects to multiple sources and performs initial cleaning
•	Functions include null handling, type conversion, and data validation

4. Data Transformation Layer
•	DAX (Data Analysis Expressions) used for KPI and metric calculations:
o	MTD/MOM Applications
o	Funded Amount
o	Average Interest Rate
o	Average DTI
o	Good vs. Bad Loan Ratio
•	M Language (Power Query) used for ETL and transformation logic

5. Data Model Layer
•	Built using a Star Schema structure:
o	Fact Table: Loan Transactions (funded, received, interest rate, DTI)
o	Dimension Tables: Borrower, Purpose, State, and Date
•	One-to-many relationships established from dimensions to fact table

6. Visualization Layer
•	Built using Power BI visuals:
o	KPI Cards → Loan Applications, Funded Amount
o	Bar/Column Charts → Applications by Purpose or Term
o	Pie/Donut Charts → Home Ownership Distribution
o	Line Charts → Monthly Trends
o	Tables → Detailed loan-level data
•	Tabs: Summary, Overview, and Details

7. Publishing & Access Layer
•	Dashboard published to Power BI Service / Workspace
•	Scheduled Refreshes ensure up-to-date reporting
•	Role-Based Access Control (RBAC) secures sensitive borrower information
•	Shared via Power BI Web App, SharePoint, or Teams
✅ This architecture ensures a transparent, auditable, and efficient data pipeline — from raw data → insights → informed decisions.


🖼️ Dashboard Views

🔷 Summary View: Portfolio-level KPIs and trend analysis
 
🔶 Overview View: Loan performance by segment, purpose, and region
 
🔷 Details View: Transaction-level insights and borrower-level data
 

🚀 Getting Started

1️⃣  Clone the Repository
git clone https://github.com/Bimoral/bank-loan-report-summary.git

2️⃣ Set Up the Environment
•	Install Microsoft SQL Server and Power BI Desktop
•	Ensure your data source (CSV, SQL, Excel) matches the schema

3️⃣ Load and Transform Data
•	Connect your data via Power BI’s Get Data feature
•	Clean and merge using Power Query
•	Define measures using DAX
•	Refresh queries to populate visuals

4️⃣ Open the Report
•	Open the .pbix file in Power BI Desktop
•	Explore Summary, Overview, and Details tabs

5️⃣ Customize (Optional)
•	Modify visuals, filters, or KPIs (e.g., ROI, Default Rate, Recovery Rate)
•	Adjust data model as needed

6️⃣ Publish and Share
•	Publish to Power BI Service
•	Configure scheduled refresh and access permissions

💡 In Simple Terms
This project turns complex, scattered loan data into clear, interactive dashboards — helping financial institutions:

•	Reduce loan defaults
•	Strengthen credit risk management
•	Improve portfolio quality
•	Make faster, smarter lending decisions

🧠 Tech Stack

•	Power BI Desktop – Visualization & Reporting
•	Microsoft SQL Server – Data Source Integration
•	Power Query / DAX – ETL & Calculation Layer
•	Excel / CSV – Data Input Sources

📚 Need Help or Want to Collaborate?

If you’d like to explore or enhance this project:

💼 Connect on LinkedIn:www.linkedin.com/in/abimbolaaraoye
📨 Email: abimbolaolatoto@gmail.com

💬 Open an Issue in this GitHub repository
I’m happy to collaborate with professionals working on financial data analytics and business intelligence solutions.

👤 Maintainer

Abimbola Araoye
Quality Control Officer & Data Analyst with over 15 years of experience in the microfinance and financial services industry.

Expertise:

•	Regulatory Compliance (AML, KYC)
•	Credit Operations & Portfolio Risk
•	Data Analytics & Reporting
Tools: Excel | SQL | Power BI
Passion: Helping financial institutions use data to drive smarter, safer lending decisions.

