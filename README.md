# data-analyst-sujit
Data Wrangling
Project Description: Data Wrangling for Storefronts Inventory at City of Vancouver
Project Title: Data Wrangling for Storefronts Inventory at City of Vancouver
Objective  
The main purpose of this initiative involves performing extensive data cleansing operations to create a dependable dataset which will support storefront analytics activities for City of Vancouver. The project seeks to prepare storefront inventory data from multiple sources by cleaning and transforming it for better quality which will benefit future analysis and reporting needs.
Background 
Multiple sources provide City of Vancouver with storefront inventory data through sales transactions and storefront service interactions and marketing campaigns. The analysis of this data becomes problematic because it comes from various sources and cannot be easily processed into useful information. The process of preparing data for analysis will lead to enhanced decision-making capabilities and improved retail performance optimization specifications.
Dataset 
The data wrangling process involves various datasets, which includes :
• Metrics data: Transaction records that include storefront IDs, purchase amounts, etc
• Transaction details: Demographic details of storefronts inventory
• Transformation logs: Logs of storefronts inquiries, and various resolutions.
• User interaction data: Email and campaign response data
Methodology
1.	Data Collection 
-	Retriving data from AWS S3 buckets along with data found in the AWS Glue Catalog.
-	Ensure datasets are relevant and metrics data from storefronts inventory.
2.	Data Assessment
-	The project utilized AWS Glue Catalog to determine data types which included Parquet and CSV and JSON formats.
-	Glue Crawlers allow the verification of schemas along with inferred metadata.
3.	Data Cleaning
-	The project solved schema inconsistency problems by implementing transformations within AWS Glue.
-	Standardization of naming conventions and duplicate removal were done.

4.	Data Transformation
-	Visual development in Glue Studio enabled creating aggregation, filtering and normalization transformations.
-	Schema types were converted while the datasets were prepared for their final output stage.
5.	Data Consolidation
-	Merging of data sources into various unified datasets.
-	Databrew jobs were leveraged for processing and loading the final cleaned datas.
6.	Documentation and Validation
-	AWS Athena was used for query validations.
-	Transform the graph of the various datas.

Tools and Technologies
-	AWS Glue Studio (Visual ETL, Crawlers, Tables)
-	AWS S3 for dataset storage and processing output
-	AWS Athena for querying transformed datasets
-	AWS DataBrew for recipe job creation and processing
-	AWS KMS for encryption and bucket security
-	Python/SQL within Glue and Athena for data validation
Deliverables 
-	The dataset exists in three formats which are CSV, Parquet and JSON alongside transformation and cleaning processes.
-	Proof of the data processing involves screenshots representing job graphs together with S3 paths alongside Athena queries.
-	The entire process from extraction through to output has been documented with a clear methodology.
Timeline
-	Expected completion of project : 4 weeks including transformations, crawling and other export stages.
The fundamental purpose of data preparation during this project is to create a standardized analytical dataset from irregular unstructured City of Vancouver data sources. The project succeeds in producing reliable unified data through its work which includes cleaning and transforming and integrating numerous storefronts inventory datasets. The prepared data permits accurate analysis leading to improved decision-making and helps facilitate efficient data governance. These steps create a base that leads to significant customer understanding as well as operational insights.
Data Quality Control
Project Description: Data Quality Control Initiative at City of Vancouver – storefronts inventory
Project Title: Implementation of Data Quality Control Measures at City of Vancouver – storefronts inventory
Objective
The City of Vancouver – storefronts inventory needs to establish a complete Data Quality Control (DQC) framework to maintain consistent enterprise data quality for better decision-making.
Background
The quality control system employed as part of the AWS Glue project discovered various data quality problems among different datasets. The collected datasets contained duplicate rows along with inconsistent formats which led to inconsistent outputs. The designed quality control system receives incoming storefront data possessions then directs valid data to S3 buckets while routing failed data to clearly marked error folders.
Scope
-	Data Profiling : It was performed using AWS Glue Data quality node and dataset selection components.
-	Data Cleansing : The implementation of schema enforcement with conditional filters became my responsibility for Glue workflows.
-	Data Validation : A visual rule-based router in AWS Glue divided data between failed records and successful records.
-	Monitoring : Data logs are integrated through CloudTrail and S3 replication dashboards.
-	Training and Awareness : The provided screenshots confirm Glue Studio enables recurring job development while delivering training to users.
Methodology
1.	Current State Assessment
-	The process of profiling began with datasets located in multiple S3 buckets using AWS Glue.
-	Input primary source from buckets.
2.	Data Profiling
-	The system employed Glue’s “Data Quality Check” and schema standardization to evaluate and clean raw input data.
3.	Establish Data Quality Metrics
-	The outcomes from Glue jobs determine the direction of data – successful records go to “Passed” while unsuccessful ones end up in “Failed.”

4.	Data Cleansing
-	Used schema validations together with transformations that either corrected data errors or removed invalid records.
5.	Validations
-	Implemented conditional routing that split data through a route selection procedure based on quality results.
6.	Monitoring and Reporting
-	Platform sfi-MCR in CloudWatch provided dashboard monitoring for bucket utilization and job performance status.
-	The event tracking functionality and trail validation capability belonged to CloudTrail.
7.	Training and Best Practices
-	The system enables users to create easily repeatable workflows which can be documented for future use.
-	The system relies on versioning along with replication to create backups of S3 data while reducing potential risks.
8.	Feedback
-	Automatic changes to schemas occurred after analysts reviewed job results along with replication status to enhance performance.
Tools and Technologies
-	AWS Glue Studio (visual ETL pipelines and schema enforcement)
-	AWS S3 (bucket management, versioning, encryption)
-	AWS CloudWatch (dashboard metrics)
-	AWS CloudTrail (event history tracking)
-	AWS Key Management Service (for data security)
-	Python/SQL (used indirectly through Glue and Athena)
Deliverables
-	Quality control Glue job with output flow for different passed and failed datasets.
-	Secured and versioned S3 buckets with enabled bucket replications.
-	CloudWatch supports monitoring of reports while CloudTrail tracks events.
-	The document includes visual components and screenshot representations displaying the entire workflow sequence with its data movement path.
Timeline
-	Expected completion of project : 4 weeks including monitoring configuration, testing and validation.
The Data Quality Control project exists to verify that City of Vancouver storefront inventory data upholds four main data quality requirements of accuracy while being complete and consistent and reliable. The data moves into separate buckets for future use or correction after passing through quality control measures that combine AWS Glue jobs and conditional routing and rule-based validation. The quality control system strengthens data reliability while making it ready for analytical purposes and operational use and compliance requirements.
 



