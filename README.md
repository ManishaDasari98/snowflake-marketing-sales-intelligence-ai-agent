# 🏦 Snowflake Marketing Sales Intelligence AI Agent
 End-to-End Data Engineering Pipeline using Snowflake Cortex AI


## 🛠️ Technology Stack

![Snowflake](https://img.shields.io/badge/Snowflake-29B5E8?style=for-the-badge&logo=snowflake&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=postgresql&logoColor=white)
![Snowflake Cortex AI](https://img.shields.io/badge/Snowflake_Cortex_AI-8A2BE2?style=for-the-badge)
![Dynamic Tables](https://img.shields.io/badge/Dynamic_Tables-FF9800?style=for-the-badge)
![Cortex Search](https://img.shields.io/badge/Cortex_Search-00A86B?style=for-the-badge)
![AI Agents](https://img.shields.io/badge/AI_Agents-E91E63?style=for-the-badge)

## 📌 Project Overview

This project focuses on building an end-to-end data engineering pipeline and AI-powered business intelligence solution using Snowflake.

The solution integrates structured and unstructured data from sales, marketing campaigns, social media mentions, and customer support cases.

Snowflake Cortex AI is used to analyze customer feedback through sentiment analysis and text classification. Dynamic Tables automate the enrichment process, while Semantic Views, Cortex Analyst, and Cortex Search enable business users to interact with the data through a Snowflake Intelligence Agent.

The objective is to transform raw business data into actionable insights using automated data pipelines and Generative AI.

## 🏗️ Project Architecture

**1. 📂 Data Sources**  
Sales | Products | Marketing | Social Media | Support Cases

         ⬇️

**2. 📥 Data Ingestion**  
Snowflake Stages + COPY INTO

         ⬇️

**3. 🗄️ Data Storage**  
Snowflake Database + Tables

         ⬇️

**4. 🤖 AI Enrichment**  
Cortex AI + Dynamic Tables

         ⬇️

**5. 📊 Analytics & Retrieval**  
Semantic View + Cortex Analyst + Cortex Search

         ⬇️

**6. 🧠 AI Agent**  
Snowflake Intelligence

         ⬇️

**7. 👥 Business Users**  
Natural-language Questions + Actionable Insights

## 🔄 Project Pipeline Flow

1. **Data Sources** → Provides sales, products, marketing, social media & support case data. 
2. **Snowflake Stages** → Stores and ingests raw CSV files using Snowflake stages. 
3. **Snowflake Tables** → Stores structured and unstructured business data.
4. **Cortex AI + Dynamic Tables** → Performs AI-powered sentiment analysis and classification, with automated data enrichment. 
5. **Semantic View + Cortex Analyst + Cortex Search** → Enables business-friendly analytics, natural-language queries and text-based information retrieval.
6. **Snowflake Intelligence Agent** → Uses Cortex Analyst and Cortex Search to answer natural-language questions and deliver actionable business insights.

## Repository Structure

```text
Snowflake-Marketing-Sales-Intelligence-AI-Agent/
│
├── .gitignore
├── LICENSE
├── README.md
├── setup.sql
├── marketing_campaigns.yaml
│
└── data/
    ├── marketing_campaign_metrics.csv
    ├── products.csv
    ├── sales.csv
    ├── social_media.csv
    └── support_cases.csv
```

**Important files:**

- `README.md` – Project overview, architecture, technologies, and implementation steps.
- `setup.sql` – SQL script for creating Snowflake objects, stages, tables, integrations, and loading data.
- `marketing_campaigns.yaml` – Semantic model containing business definitions, relationships, and verified queries.
- `.gitignore` – Specifies files and folders that Git should ignore.
- `LICENSE` – Defines the terms under which the project can be used and distributed.
- `data/` – Contains the project datasets, if maintained locally in the repository.

## ⚙️ Step-by-Step Implementation 

### Step 1: Snowflake Environment Setup 

- Create a custom administrative role.

- Configure a virtual warehouse.

- Create database and schema.

- Configure CSV file formats.

- Create external stages.

- Configure required integrations and permissions.

        Database: DASH_DB_SI

        Schema: RETAIL

        Warehouse: DASH_WH_SI

- Role: SNOWFLAKE_INTELLIGENCE_ADMIN

### Step 2: Data Ingestion

- Upload source CSV files.

- Create Snowflake tables.

- Load data using COPY INTO.

- Verify successful ingestion.

- Perform initial data validation.

### Step 3: Data Quality Checks

- Perform data quality validations.

- Record count validation.

- Null value checks.

- Duplicate record identification.

- Date format validation.

- Product identifier validation.

- Sales amount validation.

### Step 4: AI-Based Data Enrichment

Apply Snowflake Cortex AI functions to customer support transcripts.

## Functions used:

- AI_SENTIMENT: Identifies positive, negative, neutral and mixed customer sentiment.

- AI_CLASSIFY: Classifies customer issues into categories such as returns, quality and shipping.

- AI_SUMMARIZE: Generates concise summaries of support conversations.

- AI_EXTRACT: Extracts relevant information from unstructured text.

### Step 5: Automated Processing Using Dynamic Tables

- Create Dynamic Tables to automate AI enrichment.

- The enriched data includes customer sentiment and issue classification.

- Configure target lag and warehouse settings to control refresh behavior.

### Step 6: Semantic Layer Development

- Create a Semantic View to map technical database structures to business terminology.

- Define dimensions, facts, primary keys and relationships.

- This enables business users to query the underlying data using natural language.

### Step 7: Cortex Search Configuration

- Create a Cortex Search Service to retrieve relevant information from customer support data.

- Enable retrieval of relevant customer feedback and support cases.

### Step 8: AI Agent Development

- Create a Snowflake Intelligence Agent and configure.

- Cortex Analyst for structured data analytics.

- Cortex Search for unstructured information retrieval.

- Custom tools for additional business operations.

- Configure agent instructions, descriptions and example questions.

### Step 9: Security and Governance

- Implement enterprise security controls.

- Role-Based Access Control.

- Role-specific privileges.

- Dynamic Data Masking.

- Controlled access to sensitive business metrics.

### Step 10: End-to-End Validation

- Test the AI Agent using business questions and verify.

- Correct tool selection.

- SQL generation and query results.

- Retrieval of relevant support information.

- Accuracy of AI-generated insights.

- Role-based access restrictions.

**Reference:** [Snowflake – Getting Started with Snowflake Intelligence](https://www.snowflake.com/en/developers/guides/from-zero-to-agents/)
