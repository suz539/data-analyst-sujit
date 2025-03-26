# data-analyst-sujit
from docx import Document
from docx.shared import Inches

# Create a new Document
doc = Document()
doc.add_heading('BUSI 653: Cloud Computing Projects Summary', 0)

# Project 1: Data Wrangling
doc.add_heading('Data Wrangling', level=1)
doc.add_paragraph("""
Project Description: Data Wrangling for Customer Analytics at XYZ Company
Project Title: Data Wrangling for Enhanced Customer Analytics at XYZ Company

Objective: The primary goal of this project is to perform comprehensive data wrangling to prepare a robust dataset for customer analytics at XYZ Company. By cleaning, transforming, and consolidating data from various sources, the project aims to enhance the accuracy and usability of customer data for subsequent analysis and reporting.

Background: XYZ Company has accumulated customer data from multiple channels, including sales transactions, customer service interactions, and marketing campaigns. However, this data is often inconsistent, incomplete, or fragmented, making it challenging to derive meaningful insights. Effective data wrangling will facilitate better decision-making and more targeted marketing strategies.

Dataset: The data wrangling process will involve various datasets, including:
• Sales Data: Transaction records that include customer IDs, purchase amounts, product details, and timestamps.
• Customer Information: Demographic details such as age, gender, location, and account creation date.
• Customer Service Records: Logs of customer inquiries, complaints, and resolutions.
• Marketing Interaction Data: Email and campaign response data, including open rates and click-through rates.

Methodology:
1- Data Collection:
   • Gather datasets from sources such as AWS S3 buckets and AWS Glue Catalog.
   • Ensure datasets are relevant, such as `cv-sfi-trfuser`, `cv-sfi-trfretail-cate`, and metrics from Vancouver storefront data.

2- Data Assessment:
   • Identified data types including Parquet, CSV, and JSON format using AWS Glue Catalog.
   • Verified schemas and inferred metadata using Glue Crawlers.

3- Data Cleaning:
   • Addressed schema inconsistency through transformations in AWS Glue Studio.
   • Removed duplicates and standardized naming conventions.

4- Data Transformation:
   • Performed transformation logic visually in Glue Studio to aggregate, filter, and normalize datasets.
   • Converted schema types and prepared final datasets for output.

5- Data Consolidation:
   • Merged data sources into unified datasets in S3 (e.g., summarized outputs to city-semi-ds/user path).
   • Leveraged DataBrew jobs (e.g., `city-semi-job-suj`) to process and load final cleaned files.

6- Documentation and Validation:
   • Query validation was done using AWS Athena (e.g., SQL count from `cv-sfi-trfuser`).
   • Transformation graph and validation screenshots were captured as proof of steps.

Tools and Technologies:
• AWS Glue Studio (Visual ETL, Crawlers, Tables)
• AWS S3 for dataset storage and processing output
• AWS Athena for querying transformed datasets
• AWS DataBrew for recipe job creation and processing
• AWS KMS for encryption and bucket security
• Python/SQL within Glue and Athena for data validation

Deliverables:
• A cleaned and transformed dataset available in CSV, Parquet, and JSON format.
• Screenshots of job graphs, S3 paths, and Athena queries validating the process.
• Documented methodology of each stage from extraction to output.

Timeline:
• Completion of the wrangling phase: ~6 weeks, including crawling, transformation, and export stages.
""")

# Project 2: Data Quality Control
doc.add_heading('Data Quality Control', level=1)
doc.add_paragraph("""
Project Description: Data Quality Control Initiative at ABC Enterprises
Project Title: Implementation of Data Quality Control Measures at ABC Enterprises

Objective: To establish a comprehensive Data Quality Control (DQC) framework at ABC Enterprises to ensure accuracy, consistency, and completeness of enterprise data for improved decision-making.

Background: As part of the AWS Glue project, quality issues were encountered across different datasets. These included duplicate rows, format discrepancies, and inconsistent outputs. A quality control system was designed to handle incoming storefront data and route quality-passed data to validated S3 buckets and failed data to separate error folders.

Scope:
• Data Profiling: Performed using AWS Glue Data Quality node and dataset selection components.
• Data Cleansing: Handled schema enforcement and conditional filters in Glue workflows.
• Validation: Used a visual rule-based router in AWS Glue to split failed and passed data.
• Monitoring: Integrated data logs with CloudTrail and S3 replication dashboards.
• Training and Awareness: Screenshots suggest repeatable job creation in Glue Studio, training exposure.

Methodology:
1- Current State Assessment:
   • Datasets stored across various S3 buckets and initially profiled using AWS Glue.
   • Primary input source: storefront inventory from `city-of-vancouver-trf-suj` bucket.

2- Data Profiling:
   • Evaluated and cleaned raw input using Glue’s “Data Quality Check” and schema standardization.

3- Establish Data Quality Metrics:
   • Based on Glue job outcomes – passed records logged to “Passed” folder, failed to “Failed.”

4- Data Cleansing:
   • Applied schema validations and transformations to repair or exclude malformed data.

5- Validation:
   • Used conditional routing to split datasets depending on quality outcome.

6- Monitoring and Reporting:
   • Dashboard in CloudWatch (sfi-MCR) monitored bucket usage and job health.
   • CloudTrail tracked event logs and trail validations.

7- Training and Best Practices:
   • Workflows built with visual repeatability for future use and documentation.
   • Emphasis on versioning and replication to backup S3 data and mitigate risks.

8- Feedback Loop:
   • Based on job results and replication status – adjustments were made to improve schemas.

Tools and Technologies:
• AWS Glue Studio (visual ETL pipelines and schema enforcement)
• AWS S3 (bucket management, versioning, encryption)
• AWS CloudWatch (dashboard metrics)
• AWS CloudTrail (event history tracking)
• AWS Key Management Service (for data security)
• Python/SQL (used indirectly through Glue and Athena)

Deliverables:
• Quality control Glue job `city-sfi-QC-suj` with output flow for passed and failed datasets.
• Secure and versioned S3 buckets (e.g., city-of-vancouver-trf-suj) with bucket replication enabled.
• Monitoring reports via CloudWatch and event logs via CloudTrail.
• Visuals and screenshots showing all workflow stages and data routing.

Timeline:
• Estimated project duration: 8 weeks including monitoring configuration, testing, and validation.
""")

# Save document
doc_path = "/mnt/data/BUSI653_CloudComputing_Project1_2_SujitMaharjan.docx"
doc.save(doc_path)

doc_path
