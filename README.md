Healthcare Analytics Dashboard 🏥












An end-to-end healthcare analytics application designed to analyse patient wait times, hospital capacity utilisation, and healthcare risk indicators.

The platform integrates data engineering pipelines, machine learning analytics, and an interactive Streamlit dashboard that can run locally or on Databricks Compute environments to support operational healthcare insights.

⚠️ DISCLAIMER: This project is intended for analytics and research purposes only and does not provide medical diagnosis or treatment recommendations.

✨ Key Features
📊 Healthcare Analytics Dashboard

Interactive dashboard built with Streamlit providing operational insights including:

Patient waiting list monitoring

Specialty-level healthcare analytics

Hospital capacity utilisation analysis

Patient risk segmentation

Operational performance dashboards

Interactive visualisations are created using Plotly.

⚙️ Data Engineering Pipeline

Healthcare datasets are processed through scalable analytics pipelines.

Pipeline capabilities include:

Data ingestion

Data validation and transformation

Feature engineering

Analytical dataset preparation

Processing frameworks:

PySpark

Pandas

🤖 Machine Learning Analytics

Machine learning models generate healthcare insights including:

Patient readmission risk analysis

Cancellation risk monitoring

Operational trend analysis

Healthcare cost estimation

Libraries used:

Scikit-learn

XGBoost

MLflow for experiment tracking

☁️ Databricks Compatibility

The application can run within Databricks environments using Streamlit Apps.

Capabilities include:

Distributed data processing with PySpark

Scalable analytics workflows

MLflow experiment tracking

Integration with Databricks compute resources

📸 Dashboard Preview
Overview Dashboard

This view provides a high-level summary of healthcare operational metrics.

Key metrics displayed:

Total patient count

Average wait time

High-risk patient monitoring

Total healthcare cost estimates

AI-Powered Query Interface

The dashboard includes a natural language query interface allowing users to interact with healthcare data.

Example queries:

What is the average wait time for Orthopedics?
Show high risk patients with readmission risk above 70%
What is the cost impact for Cardiology?
Impact of baseline capacity 200 and capacity increase by 20%

Capabilities include:

Natural language analytics queries

Automated insight generation

Query suggestions and autocomplete

Medical terminology search functionality

🏗️ System Architecture
                ┌──────────────────────────┐
                │   Streamlit Dashboard    │
                │        (app.py)          │
                └─────────────┬────────────┘
                              │
                 ┌────────────▼─────────────┐
                 │  Analytics & ML Layer    │
                 │  ML Models + Analytics   │
                 │ model_serving_utils.py   │
                 └────────────┬─────────────┘
                              │
                 ┌────────────▼─────────────┐
                 │ Data Processing Pipeline │
                 │ Pandas / PySpark         │
                 └────────────┬─────────────┘
                              │
                 ┌────────────▼─────────────┐
                 │ Healthcare Dataset       │
                 │ CSV / Databricks Storage │
                 └──────────────────────────┘
📁 Project Structure
Healthcare_Analytics_App/
│
├── app.py                     # Streamlit dashboard application
├── model_serving_utils.py     # Data pipeline and ML utilities
├── requirements.txt           # Python dependencies
├── app.yaml                   # Streamlit deployment configuration
├── images
│   ├── dashboard_overview.png
│   └── ai_query_interface.png
└── README.md
🚀 Running the App in Databricks
Prerequisites

Databricks workspace

Databricks compute cluster or serverless compute

Streamlit Apps enabled in Databricks

Step 1 — Upload Project

Upload project files to Databricks Workspace.

Workspace → Create Folder → Upload Files

Upload the following files:

app.py

requirements.txt

app.yaml

model_serving_utils.py

dataset files

Step 2 — Deploy Streamlit App

Navigate to Compute → Apps / Streamlit Apps

Click Create App

Select the project folder

Set entry point:

app.py

Select compute (cluster or serverless)

Click Deploy

Access the Application

After deployment the dashboard becomes available through a Databricks application URL.

🧪 Technology Stack
Layer	Technology
Programming Language	Python
Data Processing	PySpark, Pandas
Machine Learning	Scikit-learn, XGBoost
Experiment Tracking	MLflow
Dashboard	Streamlit
Visualization	Plotly
Platform	Databricks Compatible
📊 Example Analytics Use Cases

The application supports several healthcare analytics scenarios:

Patient waiting list monitoring

Hospital capacity planning

Workforce demand estimation

Patient risk segmentation

Operational healthcare analytics

📈 Data Engineering Highlights

This project demonstrates several modern data engineering capabilities:

Data transformation pipelines using PySpark and Pandas

Healthcare analytics dataset preparation

Machine learning integration within analytics workflows

Interactive Streamlit dashboards for data exploration

Deployment of analytics applications on Databricks compute
