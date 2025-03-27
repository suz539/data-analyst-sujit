# data-analyst-sujit
# Data Wrangling for Storefronts Inventory at City of Vancouver

## Project Description
**Project Title:** Data Wrangling for Storefronts Inventory at City of Vancouver

### Objective
The main purpose of this initiative involves performing extensive data cleansing operations to create a dependable dataset which will support storefront analytics activities for the City of Vancouver. The project seeks to prepare storefront inventory data from multiple sources by cleaning and transforming it for better quality, which will benefit future analysis and reporting needs.

### Background
Multiple sources provide the City of Vancouver with storefront inventory data through sales transactions, service interactions, and marketing campaigns. Analysis of this data becomes problematic because it comes from various sources and cannot be easily processed into useful information. The process of preparing data for analysis will lead to enhanced decision-making capabilities and improved retail performance optimization.

### Dataset
The data wrangling process involves various datasets, including:
- **Metrics data:** Transaction records that include storefront IDs, purchase amounts, etc.
- **Transaction details:** Demographic details of storefronts inventory.
- **Transformation logs:** Logs of storefronts inquiries and various resolutions.
- **User interaction data:** Email and campaign response data.

### Methodology

#### 1. Data Collection
- Retrieved data from AWS S3 buckets along with data in the AWS Glue Catalog.
- Ensured datasets are relevant and metrics data from storefronts inventory.

#### 2. Data Assessment
- Utilized AWS Glue Catalog to determine data types including Parquet, CSV, and JSON formats.
- Glue Crawlers used to verify schemas and infer metadata.

#### 3. Data Cleaning
- Solved schema inconsistency problems via transformations in AWS Glue.
- Standardized naming conventions and removed duplicates.

#### 4. Data Transformation
- Used AWS Glue Studio for visual development to perform aggregation, filtering, and normalization.
- Converted schema types and prepared datasets for output.

#### 5. Data Consolidation
- Merged data sources into unified datasets.
- AWS DataBrew used for processing and loading final cleaned data.

#### 6. Documentation and Validation
- AWS Athena used to validate queries.
- Graphical transformation of datasets created.

### Tools and Technologies
- AWS Glue Studio (Visual ETL, Crawlers, Tables)
- AWS S3 for dataset storage and output processing
- AWS Athena for querying transformed datasets
- AWS DataBrew for recipe creation and processing
- AWS KMS for encryption and bucket security
- Python/SQL within Glue and Athena for validation

### Deliverables
- Cleaned datasets in CSV, Parquet, and JSON formats.
- Screenshots showing job graphs, S3 paths, and Athena queries.
- Complete documentation of the data wrangling process from extraction to output.

### Timeline
**Expected completion:** 4 weeks (including transformations, crawling, and export stages)

# Screenshots
<img src="image 01.png">
<img src="image 02.png">
<img src="image 03.png">
<img src="image 04.png">
<img src="image 05.png">
<img src="image 06.png">
<img src="image 07.png">
<img src="image 08.png">
<img src="image 09.png">
<img src="image 10.png">
<img src="image 11.png">
<img src="image 12.png">
<img src="image 13.png">

# Data Quality Control Initiative at City of Vancouver – Storefronts Inventory

## Project Description
**Project Title:** Implementation of Data Quality Control Measures at City of Vancouver – Storefronts Inventory

### Objective
To establish a comprehensive Data Quality Control (DQC) framework to maintain consistent enterprise data quality and support better decision-making.

### Background
As part of the AWS Glue project, various data quality issues were discovered including duplicate rows and inconsistent formats. The DQC system routes valid data to S3 buckets and invalid data to marked error folders for correction.

### Scope
- **Data Profiling:** Performed using AWS Glue Data Quality node.
- **Data Cleansing:** Schema enforcement with conditional filters in Glue workflows.
- **Data Validation:** Rule-based router in AWS Glue divided passed and failed data.
- **Monitoring:** Integrated through CloudTrail and S3 dashboards.
- **Training:** Glue Studio enables recurring job development and training support.

### Methodology

#### 1. Current State Assessment
- Profiled datasets from multiple S3 buckets using AWS Glue.
- Identified primary data sources.

#### 2. Data Profiling
- Employed Glue’s Data Quality Check to evaluate and clean raw data.

#### 3. Establish Data Quality Metrics
- Based on Glue job results, records routed as “Passed” or “Failed”.

#### 4. Data Cleansing
- Applied schema validations and data transformations to correct or remove invalid records.

#### 5. Validations
- Conditional routing enabled splitting data based on quality results.

#### 6. Monitoring and Reporting
- CloudWatch dashboards monitored bucket utilization and job performance.
- CloudTrail tracked event history and validation.

#### 7. Training and Best Practices
- Created reusable workflows with versioning and replication for S3 data backups.

#### 8. Feedback
- Analysts reviewed results and updated schemas to improve system performance.

### Tools and Technologies
- AWS Glue Studio (ETL pipelines and schema enforcement)
- AWS S3 (management, versioning, encryption)
- AWS CloudWatch (metrics monitoring)
- AWS CloudTrail (event tracking)
- AWS KMS (data security)
- Python/SQL (via Glue and Athena)

### Deliverables
- Glue jobs with outputs showing passed/failed data.
- Versioned and secured S3 buckets with replication.
- CloudWatch and CloudTrail dashboards.
- Visual documentation with screenshots of workflow sequences and data paths.

### Timeline
**Expected completion:** 4 weeks (including monitoring setup, testing, and validation)

# Screenshot
<img src="Picture 01.png">
<img src="Picture 02.png">
<img src="Picture 03.png">
<img src="Picture 04.png">
<img src="Picture 05.png">
<img src="Picture 06.png">
<img src="Picture 07.png">
<img src="Picture 08.png">
<img src="Picture 09.png">
<img src="Picture 10.png">
<img src="Picture 11.png">
<img src="Picture 12.png">
<img src="Picture 13.png">
<img src="Picture 14.png">
<img src="Picture 15.png">
<img src="Picture 16.png">
<img src="Picture 17.png">
<img src="Picture 18.png">
<img src="Picture 19.png">


> This project created standardized and unified analytical datasets from previously inconsistent and scattered sources. The wrangling and quality control measures enhance data reliability, allowing for accurate analytics, stronger governance, and improved decision-making for the City of Vancouver storefront inventory operations.
 



