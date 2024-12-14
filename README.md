# Exploratory Data Analysis

![EDA analysis](/images/eda.png)

**Project Description:**
Analyzing water system operating permits for patterns, trends, and anomalies in issued permits across mechanical system types, compliance, and contamination levels.

**Project Title:**
Exploratory Analysis of Water System Operating Permits

**Objective:**
To identify trends in permit issuance, voluntary compliance, and contamination metrics for improving regulatory focus and operational priorities.

**Dataset:**
472 entries detailing operating permits for water systems, including mechanical system types, compliance status, geographical data, contamination metrics, and renewal dates.

**Methodology:**

- Perform descriptive statistics (means, medians, frequencies).
- Visualize data with histograms, scatter plots, and trend charts.
- Identify missing data, anomalies, and correlations between variables.

**Tools and Technologies:**
- AWS Data Brew for data profiling
- AWS Glue for ETL pipeline
- Amazon S3 for data storage
- Visualization tools (e.g., Excel or Matplotlib)

**Deliverables:**
- Summary statistics
- Visualizations of permit trends and contamination data
- Insights into compliance and system types

# Descriptive Analysis

![Descriptive analysis](/images/description.png)

**Project Description:**
Summarizing the characteristics of water system permits and their distribution across system types and compliance status.

**Project Title:**
Descriptive Analysis of Water Permit Issuance

**Objective:**
To understand the distribution of permits across system types and voluntary vs. non-voluntary compliance categories.

**Dataset:**
Details 472 water systems, focusing on system types like Cooling Towers, Building Water Treatment Systems, and Decorative Water Features.

**Methodology:**
- Count and percentage distribution of permits per system type.
- Assess compliance participation rates.
- Generate bar charts for voluntary and non-voluntary permit distribution.

**Tools and Technologies:**
- AWS Athena for querying permit data
- Excel and Tableau for visualization

**Deliverables:**
- Percentage of Cooling Tower permits (55.89%)
- Charts showing compliance trends and system breakdown

# Diagnostic Analysis

![Diagnostic Analysis](/images/diagnostic.png)

**Project Description:**
Analyzing factors affecting permit renewal patterns and voluntary compliance among mechanical system types.

**Project Title:**
Diagnostic Analysis of Permit Renewal Patterns

**Objective:**
To diagnose reasons behind peak renewal periods and low voluntary compliance participation.

**Background:**
The dataset reveals a dominance of Cooling Towers in permit issuance and a peak renewal trend in 2025. Voluntary compliance remains minimal despite the critical role of Cooling Towers.

**Dataset:**
Permit records with renewal dates, compliance status, and contamination metrics.

**Methodology:**
- Query data for renewal trends in 2024-2026.
- Assess correlation between compliance and system types.
- Investigate contamination metrics and their relationship with compliance.

**Tools and Technologies:**
- AWS Glue for data pipelining
- Amazon S3 for data storage
- Tableau for trend visualization

**Deliverables:**
- Renewal trend analysis for 2025
- Factors influencing compliance

**Timeline:**
- Data extraction: 1 week
- Analysis and visualization: 2 weeks
- Report generation: 1 week

  
# Data Wrangling

![Data Wrangling](/images/wrangling.png)

**Project Description:**
Cleaning and transforming water system permit data for accurate analysis and visualization.

**Project Title:**
Data Wrangling for Water System Permits

**Objective:**
To prepare a clean and structured dataset for analysis and ensure data quality.

**Background:**
Initial data contains missing contamination metrics and whitespace issues in numerical columns.

**Dataset:**
Raw dataset stored in S3 bucket with 472 permit records.

**Methodology:**
- Profile data using AWS Data Brew.
- Clean missing values and whitespace using Data Glue recipes.
- Transform and store cleaned data in S3.

**Tools and Technologies:**
- AWS Data Brew for profiling
- AWS Glue for ETL tasks
- S3 buckets for storage

**Deliverables:**
- Cleaned dataset in S3
- Data cleaning recipes

**Timeline:**
- Data profiling: 2 days
- Data cleaning: 5 days
- Storage and validation: 2 days

# Data Quality Control

![Data Quality Control](/images/qualityControl.png)

**Project Description:**
Ensuring the reliability and accuracy of permit data through validation and governance measures.

**Project Title:**
Data Quality Control for Permit Issuance Records

**Objective:**
To validate and maintain data quality through governance frameworks and security mechanisms.

**Background:**
Data quality issues, such as incomplete contamination metrics, hinder comprehensive analysis. Steps for governance and protection are critical.

**Scope:**
Focus on improving data reliability for exploratory and diagnostic analysis.

**Methodology:**
- Create pipelines for quality assessment and segregation of passed/failed data.
- Implement encryption and replication rules in S3 for data protection.
- Monitor data quality metrics using AWS CloudWatch.

**Deliverables:**
- Quality-assured datasets
- Reports on passed/failed data
- Encrypted and replicated datasets

**Timeline:**

- Pipeline creation: 1 week
- Data governance setup: 3 days
