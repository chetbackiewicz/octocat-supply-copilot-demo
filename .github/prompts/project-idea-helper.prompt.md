---
mode: agent
description: "Help users generate a plan to create a small hackathon project that can be completed within an hour using local/mocked versions of their familiar technologies"
tools: ['codebase', 'usages', 'changes', 'githubRepo', 'search', 'create_issue', 'get_issue', 'fetch']
---

# 🚀 Project Idea Helper - Local Hackathon Projects

## 📝 Before Running This Prompt

**Customize the following sections with your preferences:**

### 🛠️ Technologies I'm Familiar With
Replace the examples below with technologies you know and want to practice:

**Technologies:**
- Terraform (Infrastructure as Code)
- Docker (Dependency management & encapsulation)
- MWAA - Airflow (Orchestration)
- DBT (Data transformation for AWS Redshift)
- AWS Batch (Compute layer)
- AWS Kinesis (Real-time streams)
- Databricks & Apache PySpark (High volume datasets & streaming)
- Healthchecks.io (Monitoring)
- PagerDuty (Alerting)

**Programming Languages:**
- Python (All integration and code logic)
- SQL (Data transformation)

### 🎯 Problem Areas I Want to Practice (Optional)
Replace with areas you want to improve or commonly face challenges in:

- Data processing and ETL pipelines
- Real-time data streaming
- Infrastructure automation
- Data transformation and modeling
- Workflow orchestration
- Monitoring and alerting
- Containerized applications

## 🎯 Objective

Generate a **1-hour hackathon project** that:
- Uses **local, free alternatives** to your familiar technologies
- Can be run entirely on a local machine without external dependencies
- Provides hands-on practice with core concepts
- Includes specific Copilot prompts to accelerate development

## 📋 Project Requirements

### ✅ Must-Haves:
- **Runnable locally** - No cloud accounts, APIs, or paid services required
- **Mock data** - Generate realistic sample data instead of real integrations
- **File-based** - Use local files, SQLite, or in-memory structures
- **Documented** - Clear setup and run instructions
- **Completable in 1 hour** - Focused scope with clear deliverables

### 🚫 Avoid:
- External API dependencies
- Complex infrastructure setup
- Database servers requiring installation
- Paid services or accounts

## 🔄 Technology Translation Examples

**Instead of real cloud services, suggest local alternatives:**

| Enterprise Technology | Local Alternative | Implementation |
|----------------------|-------------------|----------------|
| AWS Kinesis | File-based streaming | JSON Lines files with timestamp processing |
| MWAA/Airflow | Local Airflow | Docker Compose setup or Python scripts with cron-like scheduling |
| Terraform | Local file management | Python scripts that generate config files |
| DBT + Redshift | DBT + SQLite/DuckDB | Local DBT project with file-based database |
| AWS Batch | Local Python processes | Multiprocessing or threading for parallel tasks |
| Databricks/PySpark | Local PySpark/Pandas | Smaller datasets processed with pandas or local Spark |
| Healthchecks.io | File-based logging | JSON logs with status checks |
| PagerDuty | Local notifications | Console alerts or simple email/webhook simulation |
| Docker containers | Local processes | Multiple terminal windows/processes |
| PostgreSQL/MySQL | SQLite/DuckDB | Local database files |

## 🎨 Project Ideas Template

For each suggested project, provide:

### 📊 Project: [PROJECT_NAME]
**Concept:** Brief description of what the project does

**Technologies Practiced:**
- [Original Tech] → [Local Alternative]
- [Original Tech] → [Local Alternative]

**Architecture:**
```
[Simple ASCII diagram or bullet points showing data flow]
```

**Deliverables:**
- [ ] Component 1 (e.g., data generator script)
- [ ] Component 2 (e.g., processing pipeline)
- [ ] Component 3 (e.g., simple dashboard/output)

**Setup Instructions:**
1. Create project directory
2. Install dependencies (list specific packages)
3. Run components in order

**Copilot Prompts:**
- "Create a [specific function] that [specific task]"
- "Write a [component] that reads from [source] and outputs [format]"
- "Generate mock data for [domain] with fields [list fields]"

**Extension Ideas:**
- Add feature X for more complexity
- Integrate with local tool Y
- Create visualization with Z

## 🎲 Sample Projects

### 📈 Data Pipeline with DBT Transformation
**Mock:** Kinesis → File streaming, DBT + Redshift → DBT + SQLite, Airflow → Python scheduler
**Time:** 45-60 minutes
**Output:** Transformed sales data with DBT models and documentation

**Architecture:**
```
Raw Data (JSON) → Python Ingestion → SQLite (staging) → DBT Transform → SQLite (marts) → Reports
```

**Deliverables:**
- [ ] Mock data generator (sales_generator.py)
- [ ] Data ingestion script (ingest.py)
- [ ] DBT project with staging and mart models
- [ ] Simple orchestration script

**Copilot Prompts:**
- "Write a Python function generate_sales_data that returns a dictionary with product_id, quantity, timestamp, and customer_id"
- "Create a DBT staging model (stg_sales.sql) that cleans and casts raw sales data, handling NULL values"
- "Write a DBT mart model (fact_daily_sales.sql) that aggregates cleaned data for daily sales by product"
- "Generate schema.yml for the fact_daily_sales model with descriptions and data types"

### � Real-time Stream Processing Pipeline
**Mock:** Kinesis → File-based queue, Spark Streaming → Python + pandas, Batch → Local processing
**Time:** 45-60 minutes
**Output:** Real-time analytics dashboard with streaming data

### 🔄 Infrastructure Automation Simulator
**Mock:** Terraform → Python config generator, AWS services → Local file structures
**Time:** 30-45 minutes
**Output:** Configuration management system that generates local "infrastructure"

### � Data Quality Monitoring System
**Mock:** Healthchecks.io → Local logging, PagerDuty → Console alerts, Airflow → Python scheduler
**Time:** 45-60 minutes
**Output:** Data quality checks with alerting and reporting

### 🏪 Containerized ETL Pipeline
**Mock:** Docker → Local processes, AWS Batch → Multiprocessing, Kinesis → File streaming
**Time:** 45-60 minutes
**Output:** Multi-stage data processing pipeline with dependency management

## 💡 Generation Instructions

Based on the technologies and problem areas listed above:

1. **Analyze the input technologies** and identify local alternatives
2. **Match problem areas** to relevant project types
3. **Suggest 3-5 project options** with varying complexity
4. **Provide complete implementation plan** for the chosen project
5. **Include specific Copilot prompts** for each major component
6. **Estimate realistic timeframes** for each deliverable

Generate projects that feel authentic to the technologies they're practicing while being achievable in the time constraint.
```

