🧠 H1B Visa Status Predictor
The H1B Visa Status Predictor is a data-driven machine learning project that analyzes historical H1B visa application data to predict the outcome (approval/rejection) and provide actionable insights. The goal is to reduce uncertainty in the complex visa application process and support informed decision-making for stakeholders.

📌 Problem Statement
The H1B visa process is uncertain and critical for employers and foreign applicants. This project leverages machine learning to:

Predict visa application outcomes.

Analyze patterns and trends in past applications.

Help optimize application strategies based on historical data.

📂 Dataset
Source: Kaggle

Size: 3.5M+ records, 96 columns

Based on public disclosures from the US Department of Labor (DOL)

⚙️ Technologies Used
Python, Pandas, PySpark, Seaborn, Scikit-learn

Machine Learning

Microsoft Azure (Data Factory, Data Lake Gen2, Databricks, ML Studio, Synapse Analytics)

Streamlit (for UI)

Power BI (for dashboards and insights)

🚀 Workflow
1. Local System
Loaded data using Pandas

Performed extensive EDA (null handling, outliers, transformations)

Used Matplotlib/Seaborn for visualizations

Applied ML models using Scikit-learn

Built an interactive dashboard using Power BI

2. Azure Cloud
Used Azure Data Factory to create ETL pipelines

Stored data in Azure Data Lake Gen2

Cleaned and transformed data with Azure Databricks (Apache Spark)

Built ML models in Azure ML Studio

Queried data using Azure Synapse Analytics

Integrated dashboard with Power BI

🧹 Data Cleaning & Preprocessing
Dropped columns with >90% nulls (e.g., Employer address)

Selected key columns (~18) for analysis like Case Status, Wage, Job Title, Location, etc.

Standardized categorical entries (e.g., Y/N → Yes/No)

Converted dates and calculated Processing Time

Merged multiple yearly datasets using Pandas

📊 Key Insights
~90% of applications were certified (approved)

Processing time median: 7–8 days

Highest paid roles: CEO, COO, Director

Top hiring states: California, Texas, New York

Prevailing wage had the highest correlation with visa approval

Significant drop in applications after 2020 (COVID impact)

March had the highest application submissions

📉 Predictive Modeling
Used classification models (e.g., Random Forest)

Evaluated with classification metrics: Accuracy, Precision, Recall, F1-score

Converted Case Status to numeric for correlation analysis

Initially misapplied regression metrics (R²) but corrected to classification metrics

📈 Power BI Dashboard Highlights
Pie Chart: % of certified vs denied applications

Line Graph: Year-wise decline in applications

Bar Chart: Top job titles and states

Cards: KPIs like average salary, median processing time

Slicers & bookmarks for interactivity

☁️ Why Azure over AWS?
Better integration with Power BI and Microsoft ecosystem

Cost-effective: $200 student credits + free tier

Smoother transition between Azure services

🏁 Conclusion
This project not only builds a predictive model but also offers valuable trends and strategies for visa applicants and employers. It showcases the power of integrating cloud platforms, machine learning, and BI tools to solve real-world policy and economic problems.

📎 How to Run the Project
Clone the repo and set up Python environment

Install dependencies:

bash
Copy
Edit
pip install pandas seaborn scikit-learn streamlit
Load the merged CSV file using Jupyter/Databricks

Train models and analyze outputs

Launch Streamlit app (if included):

bash
Copy
Edit
streamlit run app.py
