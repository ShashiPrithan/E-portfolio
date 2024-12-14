**Descriptive Analysis of City of Vancouver Block Numbers**

Project Description	

Project Title

Objective

Dataset	

Methodology	

Tools and Technologies	

Deliverables

**Data Wrangling for City of Vancouver Block Numbers**

Project Description

Project Title

Objective

Background

Dataset

Methodology 

Tools and Technologies

Deliverables

Timeline

**Data Quality Control of City of Vancouver Block Numbers**

Project Description

Project Title

Objective

Background

Scope

Methodology

Deliverables

Timeline

**Descriptive Analysis of Recruitment Selection Using AWS Services**

Project Description	

Project Title

Objective

Dataset	

Methodology	

Tools and Technologies	

Deliverables

**Data Wrangling for Recruitment selection at UCW**

Project Description

Project Title

Objective

Background

Dataset

Methodology 

Tools and Technologies

Deliverables

Timeline

**Data Quality Control of Recruitment Selection at UCW**

Project Description

Project Title

Objective

Background

Scope

Methodology

Deliverables

Timeline


**Descriptive Analysis of City of Vancouver Block Numbers**

**Project Description:**

The **Descriptive Analysis of City of Vancouver Block Numbers Data** uses AWS services to examine block occurrences, trends, and geographic distributions. Data is ingested and stored in **Amazon S3**, cleaned with **AWS Glue DataBrew**, and accessed through **Athena**. The key data, including total occurrences, frequency distributions, and peak patterns, are summarized. **DynamoDB** stores segmented insights and geographical data for easy access. **Amazon QuickSight** creates visualizations such as time-series graphs and heatmaps. **CloudWatch** and **CloudTrail** provide monitoring and security, whilst **AWS KMS** protects data. Insights help with municipal planning, resource allocation, and infrastructure management.

**Project Title:** Descriptive Analysis of City of Vancouver Block Numbers Data using AWS Cloud Services.

**Objective**
The major purpose of this project is to do a thorough descriptive analysis of block number data, summarise significant statistics, discover time-based trends, and produce geographical insights. The investigation will give useful information for municipal planning, infrastructure development, and governance decisions.

**Dataset**
The dataset consists of the following important attributes:

**Geo_Local_Area:** Geographic area name (for example, Downtown, West End, etc.).

**Block_Numbers_Count:** The block numbers per geographical region.

**Label:** Classification of land use (for example, residential, business, or industrial).

**Geoms** Coordinates are geographic positions that serve as geographical references.

**Methodology:**

**Data collection and preparation.**

**Data Ingestion**
**AWS Service: Amazon S3**.
Upload raw data to the pad-bn-raw-sha S3 bucket.
To ensure data security, enable versioning and encryption using AWS KMS.
To provide redundancy, replicate data to a backup bucket (pad-bn-raw-back-sha).
To ensure security, restrict access to S3 buckets with AWS Identity and Access Management (IAM).

**Data Cleaning:**
**AWS service : Glue DataBrew service.**
**Tasks:**
Handle missing values (by imputation or removal).
Correct data types (such as timestamps and numeric fields).
Remove any duplication and inconsistencies.
Detect and manage outliers in geographic and frequency data.
The cleaned data is stored to the pad-bn-trf-sha bucket for subsequent examination.

**Metadata Management.**
**AWS Services: AWS Glue Crawler**
The purpose is to automatically catalog data stored in S3 buckets.


**Descriptive statistics.**

**AWS service: Amazon Athena.**
**Tasks:**
Query the cleaned dataset located in S3 buckets.
Calculate the key metrics:
Overall block occurrences across time.
Mean, median, and mode for block numbers.
The frequency distribution of blocks across categories.
Store summary tables in the pad-bn-cur-sha bucket.

**Data segmentation.**
**AWS Service: Amazon DynamoDB.**
Process:
Divide blocks into categories, such as:
High-Frequency Blocks are block numbers that occur frequently.
Low-frequency blocks have rare block numbers.
Geospatial characteristics should be included using a geo-indexing schema to improve query performance.

**Data Governance & Monitoring**

**Monitoring with CloudWatch**
**AWS Services: Amazon CloudWatch:**
Monitor the status of the Glue task execution, including logs and problems.
Monitor S3 bucket utilization metrics:
Storage Size (BucketSizeBytes)
Number of objects
Cost estimates for S3 and Glue based on the EstimatedCharges measure.
Dashboard: Create a customized CloudWatch dashboard to visualize metrics.

**Auditing with CloudTrail**
**AWS Services: AWS CloudTrail**
**Purpose:** Monitor user activities on S3 buckets, including data uploads and access.
AWS Glue jobs (such as job creation and execution).
IAM policy updates for data security.


**Insights and findings**
Peak Patterns: Determine the periods (e.g., months, weeks) with the highest block incidence.
Category Trends: Showcase changes in block categorization over time.
Geospatial insights: View block distribution across city areas.
High-Impact Blocks: Determine whether blocks have a high or unusual number of occurrences.


## **Recommendations**  
1. **Optimize High-Frequency Blocks**: Prioritize infrastructure improvements and maintenance in blocks with the most recurring patterns.  
2. **Improve little-Utilization Zones**: Identify and evaluate blocks with little activity in order to improve city services or reuse unused spaces.  
3. **Improve Resource Planning**: Align personnel and resource allocation with peak activity times determined by time-series patterns.  
4. **Use Geospatial Insights**: Heatmaps may be used to highlight areas prone to congestion or anomalies, allowing for improved traffic and zone management.  
5. **Implement Data Monitoring**: Validate and maintain data quality on a regular basis using **AWS CloudWatch** and scheduled **Athena** queries.  


**Tools and technologies.**

**Amazon S3:** provides storage for both the raw and sanitized datasets.

**AWS Glue:** Data catalog development and transformation tasks.

**AWS Glue DataBrew:** AWS Glue DataBrew cleans and transforms data.

**Athena:** Amazon Athena enables data querying and validation.

**Amazon DynamoDB:** Amazon DynamoDB provides storage for accident records that have been cleansed and converted.

**Cloud Watch** CloudWatch monitors Glue job activity and system performance.

**Cloud Trail** CloudTrail logs AWS activity for security and auditing purposes.

**IAM and KMS** IAM and KMS provide secure data access and encryption.


**Deliverables** 

1. **Cleaned and Consolidated Dataset**: Validated block number data securely stored in **Amazon S3**.

2. **Insight Report**: Detailed findings on block trends, peak periods, and geographic patterns for educated decisions.

3. **Monitoring Framework:** Real-time CloudWatch dashboards and Athena-based data quality tests to ensure data integrity.

4.**Actionable Recommendations:** A thorough report including plans for infrastructure upgrades, resource optimization, and zoning enhancements.

![image](https://github.com/user-attachments/assets/33f0c463-fff1-4166-b9ae-86b74cea4466)


**Data Wrangling for City of Vancouver Block Numbers**

**Project Description**
The Data Wrangling for City of Vancouver Block Numbers Data project will clean, restructure, and combine block number utilizing AWS services. After being cleaned with *AWS Glue DataBrew and converted with **AWS Glue ETL, the data is ingested into *Amazon S3. To ensure high-quality data, duplicates, missing values, and inconsistencies are rectified. *Athena is used for validation, while **DynamoDB is used to store consolidated datasets for optimal querying. Security and monitoring are guaranteed by *CloudWatch, **CloudTrail, and **AWS KMS. In order to facilitate city planning, infrastructure management, and geospatial analysis, this project produces a solid, cohesive dataset.

**Project Title:**  
Data Wrangling for Enhanced Analysis of City of Vancouver Block Numbers Data Using AWS Services

**Project Objective**
Performing thorough data wrangling on the City of Vancouver block numbers dataset in order to provide a clean, accurate, and unified dataset for analysis is the main goal of this project. Through the use of AWS services for data integration, transformation, and cleaning, the project seeks to provide trustworthy insights that assist **city planning, resource allocation, and infrastructure management. 

**Project Background**
The City of Vancouver's block numbers dataset is fragmented, inconsistent, and incomplete, including block numbers, timestamps, classifications, and geospatial coordinates. Improving the dataset's quality, consistency, and usefulness for additional research and reporting requires careful data wrangling. This procedure will guarantee that the data complies with analytical goals and city governance regulations, facilitating well-informed decision-making. 


**Dataset Description**
1. Block Number: A block's unique identification number. 
2. Timestamps: Information depending on time.
3. Categories: Block classification (e.g., business, residential). 
4. Geolocation Data: Coordinates for latitude and longitude that are used to map city blocks. 

**Methodology**

**Data Collection**
**AWS Service: Amazon S3 **
Process: 
Collect block numbers data from the source and upload it to the *pad-bn-raw-sha S3 bucket*. 
To protect the data while it is being ingested, use AWS KMS to enable versioning and server-side encryption. 
In order to prevent data loss, replicate the data to a backup bucket *pad-bn-raw-back-sha* for redundancy. 
Create a AWS Glue Crawler to categorize raw data and generate metadata automatically. 

**Data Assessment**
**AWS Services: Amazon Athena and AWS Glue**
Process: 
Athena is used to immediately execute preliminary data queries on the raw data that is stored in S3. 

Recognize and record problems with data quality, such as:
- Missing values in geolocation or timestamp fields. 
The block numbers have duplicate records. 
The date formats and categorization name conventions are inconsistent. 
Create an overview report that highlights the dataset's inconsistencies. 

**Data Cleaning**
**AWS Service: AWS Glue DataBrew**
- Tasks: 
- Managing Missing Values: 
Missing timestamps can be replaced by imputation methods (e.g., nearest available value). 
Eliminate any rows that lack important details, like block numbers. 
   - Duplicate Removal:
 Identify and remove duplicate rows for block numbers without losing vital information. 
Consistency in Data Format: 

To standardize date formats, all timestamps should be converted to ISO 8601. 
- Normalize categorical fields (for example, combine "Residential" and "Res" into a single standard category). 
Detection of Outliers: 
- Identify and manage geographic abnormalities in latitude and longitude data. 

Storage: Store the cleaned dataset for validation and further processing in the *pad-bn-trf-sha S3 bucket*. 


**AWS Service:** 
AWS Glue Data Transformation 

**Process:**
- Transform the cleansed dataset using AWS Glue ETL jobs. 
Timestamps should be converted into the proper datetime objects for time-series analysis. 
- Generate new derived fields, like: 
- Occurrence Frequency: The total number of times a block number occurs in a given week or month. 
Block Category Trends: Totals for every category. 
* Geographical Characteristics: In order to facilitate mapping, combine latitude and longitude into a single *geo_point field. 
- Combine the data into summary tables to facilitate querying and reporting. 
- Storage: For maximum flexibility, return altered data to the *pad-bn-cur-sha bucket* in both Parquet and CSV formats. 

**Data Consolidation:**
- AWS Services: AWS Glue and DynamoDB 
- Procedure: 
- Use AWS Glue ETL jobs to combine all pertinent datasets into a single, consolidated dataset. 

- Ensure that block numbers act as unique keys to appropriately link records. 
- Import aggregated datasets into Amazon DynamoDB for efficient querying and analysis. 
- Enable geo-indexing for more effective geospatial data retrieval. 


**Documentation and Validation**
AWS services include CloudWatch, CloudTrail, and Amazon Athena. 
Tasks: 
- Validate the final dataset using Athena by doing out: 
- Conduct exploratory data analysis (EDA) to ensure that the data is complete and correct. 
- Statistical tests (e.g., category distributions, block occurrence counts). 
- Record the full data wrangling procedure, including: 
- The data sources 
Methods of cleaning and transformation 
- Challenges encountered, and solutions adopted. 
* Monitoring: To keep tabs on S3 metrics and Glue job logs, use *CloudWatch. 
- Auditing: Make sure all user actions are documented for traceability by using **CloudTrail to log them. 

 **Data Security and Governance**
Data Encryption: Use AWS KMS to encrypt data both at rest (S3, DynamoDB) and in transport. 
Access Control: Implement stringent IAM roles and policies to manage access to DynamoDB, Glue, and S3 resources. 
Backup and replication:To provide redundancy and recovery, replicate S3 buckets to a backup site. 

**AWS Services and Tools**
Amazon S3: Raw, cleaned, and transformed datasets can be stored here. 
AWS Glue DataBrew: Data preparation and cleansing. 
AWS Glue: ETL tasks for integration and data transformation. 
Amazon Athena: SQL querying for exploratory analysis and validation. 
Amazon DynamoDB: Using geo-indexing to store aggregated datasets for fast access. 
AWS KMS: Data security and encryption. 
AWS CloudWatch: Tracking S3 performance and Glue job metrics. 
AWS CloudTrail: Logging and auditing for governance. 

**Deliverables**
1. Cleaned and Consolidated Dataset: An analysis-ready unified dataset that is stored in S3 and DynamoDB. 
2. Comprehensive Documentation: An in-depth account of the difficulties, strategies, and data wrangling process. 
3. Validation Results: Verification of data quality using summaries and visualizations of exploratory analysis. 
4. Monitoring Dashboard: CloudWatch dashboard for tracking data processing operations. 

**Timeline**
Week 1: Gathering and encrypting data before importing it into Amazon S3. 
Week 2: Quality tests are performed on the data using AWS Glue Crawlers and Athena. 
Week 3: Using AWS Glue DataBrew to clean the data (dealing with duplicates, missing values, and inconsistencies). 
Week 4: Data transformation using AWS Glue ETL, which includes feature engineering and aggregation. 
Week 5: Using Athena queries for validation and consolidating data in DynamoDB. 
Week 6: CloudWatch monitoring setup, documentation, and the last delivery of reports and datasets that have been cleaned.

The project will result in a high-quality, consistent, and consolidated dataset of City of Vancouver block numbers. Utilizing AWS services will optimize the data for accessibility, security, and accuracy. This will allow for the discovery of block trends, patterns, and insights that are essential for city planning, infrastructure optimization, and resource allocation through downstream analysis. AWS tools are used in the project to guarantee cost effectiveness, governance, and scalability. 


![image](https://github.com/user-attachments/assets/7b4ee584-69a3-4643-aab5-426ec86af1eb)


**Data Quality Control for City of Vancouver Block Numbers**

 **Project Description**
The objective of this project is to use AWS services to create a thorough Data Quality Control (DQC) framework for the City of Vancouver block numbers dataset. In order to guarantee data accuracy, completeness, consistency, and dependability, the project will set up procedures for data profiling, cleansing, validation, monitoring, and reporting. Among the AWS tools that will help the project manage, validate, and monitor data quality are S3, **AWS Glue, **Athena, **CloudWatch, and **KMS. The end result will be reliable data integrity, easier city planning, and better operational decision-making for infrastructure and governance improvements. 

**Project Title:**
Data Quality Control for City of Vancouver Block Numbers Using AWS Services  

**Scope of Work** 
1. Data profiling: Evaluating the accuracy, uniqueness, and completeness of the available data. 
2. Data Cleaning: Fixing mistakes, eliminating duplicates, and standardizing formats. 
3. Data Validation: Creating and enforcing validation rules to ensure data integrity. 
4. Monitoring and Reporting: Using dashboards and alerts to do real-time quality chec4. Monitoring and Reporting: Using dashboards and alerts to do real-time quality checks. 
5. Training: Providing users with instruction on recommended practices to ensure continuous data quality. 

**Methodology**

**Data Assesment**
- AWS Service: AWS Glue, Amazon S3 - Workflow: 
- Transfer the raw dataset to a S3 bucket named pad-bn-raw-sha. 
- To catalog data and find problems with data quality, such as missing values (timestamps, geolocations), use AWS Glue Crawlers. 
-The block numbers are duplicates. 
-Inconsistent formats for data (e.g., coordinates, date). 
-Create a preliminary summary report by utilizing Athena queries to gain knowledge about data irregularities. 

**Data Profiling** 
**AWS Service: AWS Glue DataBrew**

**Procedure:**
- Utilize DataBrew to assess the uniqueness, validity, and completeness of data. 
- Emphasize key features: 
Block Numbers: Look for items that are invalid or duplicated. 
Timestamps: Make sure the date and time formatting is correct. 
- Categories: Establish and validate classification values. 
- Geolocation: Determine the precision of latitude and longitude. 
Record the results of the profiling for future use. 

**Data Quality**
Define measurements and KPIs for monitoring: 
Completeness: The dataset's percentage of non-null values. 
Uniqueness: percentage of block numbers that are unique. 
Accuracy: Verification against preset thresholds and formats. 
Error Rate: The proportion of inaccurate or inconsistent data. 

- Storage: Use DynamoDB to store baseline measures and KPIs for continuing tracking. 

**Data Cleaning**
**AWS Services: AWS Glue DataBrew, AWS Glue** 
*Tasks:*  
Duplicate Removal: To find and eliminate duplicate block numbers, use **DataBrew. 
Missing Value Handling: Use imputation techniques (for example, fill with defaults or nearest neighbor). 
Data Standardization: To ensure consistency in: 
The ISO 8601 date formats. 
Coordinates in a geographic format (latitude-longitude). 
- Category values, such as "Residential" versus "Res." 
- Outlier Detection: Scan geolocations and block numbers for irregularities. 
Storage: Store the cleaned dataset in the S3 bucket designated *pad-bn-trf-sha*. 

**Procedures and Rules for Validation**
**AWS Service: AWS Glue ETL**
*Method*:
Define validation rules. 
Block Numbers: These have to be distinct and numerical. 
Timestamps: The ISO 8601 format must be used. 
Categories: Verify against a pre-established classification list. 
- Geolocations: Check for valid latitude-longitude ranges. 
- Create ETL scripts in AWS Glue to evaluate incoming data before storing it. 
- Query and verify data integrity after validation using Athena. 

**Monitoring and Reporting**
**AWS Services: Amazon CloudWatch, AWS Glue, CloudTrail, Athena**
Tasks:  
CloudWatch can be used to:
- Track metrics related to S3 storage (such as data size and error counts) and Glue job execution. 
- Create warnings in real time when KPIs are not being met. 

Use Athena to perform recurring SQL-based assessments of data quality metrics. 
CloudTrail should be enabled in order to record and audit all Glue task and S3 bucket actions. 

 **Tools and Technologies:**
Amazon S3: Safe storage for unprocessed, cleaned, and verified datasets. 
AWS Glue: Data transformation and validation jobs for validation rules and ETL. 
AWS Glue DataBrew: Cleaning and profiling data. 
Amazon Athena: SQL querying for data quality metrics analysis and validation. 
Amazon DynamoDB: KPI and baseline metrics storage. 
Amazon CloudWatch: Tracking the performance of the data pipeline and generating notifications. 
Data activity auditing and logging for governance using AWS CloudTrail. 
AWS KMS: Encrypting data to guarantee security both in transit and at rest. 

**Deliverables**
1. Comprehensive Data Quality Control Plan: Recording duties, metrics, and procedures. 
2. Cleaned and Validated Dataset: Data of superior quality, safely stored in Amazon S3. 
3. Training Resources: Stakeholder workshops and materials. 
4. Validation Reports are summaries of data quality indicators and outcomes. 


**Timeline**
Weeks 1-2: Profiling data and assessing the current state (using S3, Glue Crawlers, and DataBrew). 
Weeks 3–4: Implementing Data Cleaning and Validation Rules (with Athena and Glue ETL). 
Week 5: Process documentation and training.
Weeks 6-7: Completed Validation, Testing, and Submission of Deliverables. 

This project will guarantee the quality, completeness, and consistency of the City of Vancouver block numbers dataset by providing a strong Data Quality Control framework. Real-time monitoring dashboards and clear, verified data will enable stakeholders to maximize infrastructure planning, make well-informed decisions, and improve operational efficiency with AWS's

**Descriptive Analysis of Recruitment Selction Using AWS Services**

**Project Description**
This project analyzes recruitment and selection procedures utilizing AWS tools to increase efficiency and compliance. AWS Glue and AWS DataBrew are used to clean and transform data from referral programs, application processes, candidate management, secrecy storage, and blackout periods. The data is safely saved in Amazon S3. We use DynamoDB to manage candidate metadata. Amazon VPC and security groups are used to guarantee security. Through the use of AWS's scalable and secure cloud-based solutions, the project seeks to improve HR teams' decision-making, expedite recruitment operations, and identify patterns.

**Project Title:** Understanding Recruitment and Selection Patterns with AWS Integration

**Objective **
The primary goal of this research is to compile and analyze recruiting data, such as referral programs, application processes, candidate management, confidentially storage, and blackout periods. Amazon S3, AWS Glue, AWS DataBrew, and Amazon EC2 are used to store, analyze, and visualize data in a safe, scalable, and efficient manner.

**Dataset**
The recruitment dataset includes the following essential elements: 
1. Program for Referrals: Offers compensation for job referrals according to the type of position.
2. Application Selection Process: Determines submission procedures for various roles, including faculty, administrative staff, and students. 
3. Candidate Management: Provides information on how to notify applicants, keep track of notes, and maintain confidentiality. 
4. Confidentiality Storage: Provides guidelines for securely maintaining recruitment-related records. 


**METHODOLOGY**

**Data Collection and Storage:**
The dataset was stored in Amazon S3 as raw files for secure and scalable storage.
Amazon VPC was utilized to secure resources and manage network access to S3 data.
Security teams made sure that only individuals with permission may view the hiring information.

**Data Cleaning and Preparation:**
The dataset was cleaned and transformed using AWS Glue's ETL (Extract, Transform, Load) procedures.
We discovered and repaired missing values, corrected data types (e.g., dates, strings), and eliminated duplicate records.
To ensure that the data was prepared for descriptive analysis, AWS DataBrew was used to visually analyze and clean it.

**Descriptive Statistics**

**Referral Program**
Full-time permanent roles received the highest referral rewards, demonstrating that the organization favors secure and long-term work. The incentives for casual and part-time jobs were smaller, which was indicative of their lower organizational priority. These reward patterns were highlighted using effective data extraction made possible by AWS Glue, and the processed output was safely stored on Amazon S3. 

**Application Selection Procedure**

The submission method was explicitly established for each application type: administrative, faculty/teaching, and student. The significance of specialization was demonstrated by the professor posts' unique email channels, which we discovered by examining submission methods safely maintained in the Amazon Elastic File System (EFS). For recruitment teams across departments, file accessibility was guaranteed with Amazon Shared Location. 

**Candidate Management**
Strong adherence to HR policies was shown by the candidate management procedures: 
The following candidate management procedures showed excellent adherence to HR policies: 
• Prompt notification of non-shortlisted candidates.
• Interview notes were securely retained for one year before being destroyed. 
• The data of successful applicants was kept for a long time. 

**Data Enriching**
Candidate metadata was stored in the DynamoDB database, which allows for rapid access to structured data. This data was processed and managed at scale and in a secure manner using Amazon EC2 instances. 
Security Storage
Data privacy was managed using strong procedures: 

• Interview notes were destroyed after one year, whereas successful candidate records were kept until the job tenure ended. 
• The general candidate data met several legal standards. 
AWS features such as S3 versioning and S3 lifecycle controls ensured secure document keeping and automated deletion once expired. An additional layer of security was introduced by Amazon VPC security groups to ensure secrecy. 


**Data Visualization and Reporting**

**1. Sales and Reward Trends:** 
AWS Amazon Glue Data Brew was used to depict a time-series study of referral rewards and hiring procedures, offering insights into hiring patterns throughout the year.

**2. Candidate and Application Trends:**
o Bar charts showing the distribution of hiring kinds and application techniques were displayed.
Heatmaps were used to depict hiring trends, indicating peak and blackout periods.

**3. Confidentiality Compliance:**
Process flow diagrams provided a clear representation of document destruction procedures and retention periods.
Stakeholder accessibility was guaranteed by the secure hosting of all visualizations on Amazon Glue data brew.

**Key Insights and Findings**
1. Referral Program: The organization promotes recommendations for key full-time positions, offering higher incentives. Lower pay for casual positions indicates areas for improvement in attracting temporary personnel.
2. Application Process: Dedicated submission channels simplify the process and ensure that role-specific applications are effectively managed. 
3. Candidate Management: Compliance with data preservation and deletion standards demonstrates effective HR data governance approach. 
4. Storage of Confidentiality:AWS solutions like as S3 lifecycle policies guarantee compliant and automated document deletion, minimizing the need for human interaction. 

**Tools and Techniques**

**Amazon S3:** Secure and centralized storage for both processed and unprocessed hiring data.

**AWS Glue:** Constructed data for analysis by performing ETL procedures. 

**AWS DataBrew:** a visual interface for automated and simplified data cleaning. 

**Amazon EC2**: Scalable computing for workloads including data processing. 

**DynamoDB:** Effectively managed candidate metadata to enable speedy retrieval. 

**Amazon EFS:** File systems that are shared by recruitment and HR teams. 

**Amazon Security Groups and VPC:** Safe access to data and networks. 

**Recommendations:**
1. Strengthen Referral Programs: To increase candidate recommendations for casual and part-time positions, implement tiers of referral benefits. 
2. Streamline Application Procedures: To enhance the applicant experience, automate emails acknowledging applications received. 
3. Improve Data Governance: Use AWS technologies like S3 Glacier to archive successful applicant information and save storage expenses. 

**Deliverables**
1. A comprehensive report that provides a summary of descriptive insights, procedures, and results. 
2. Visual dashboards with interactive features made with Amazon Glue Data Brew. 
3. An architecture diagram of AWS that shows the implemented tools and procedures. 

This research provides a thorough insight of the recruitment dataset, resulting in streamlined processes, increased secrecy, and effective tactics utilizing AWS resources. 

![image](https://github.com/user-attachments/assets/5ec72ab7-196f-46de-87bf-44e3ca80f4e9)

 
 **Data Wrangling for Recruitment Selection at UCW**

**Project Description**
The project aims at preprocessing the data contained in the Recruitment Datasetby clean and transforming the data and then consolidating the data in a structured format that can be analyzed using various AWS services. Tools are amazon S3 for storage, EC2 for data preparation, AWS Glue, and AWS Glue DataBrew for profiling/ cleaning, DynamoDB and for querying structural insights an Athena. It implements continual monitoring and security features leveraging CloudWatch as well as CloudTrail; Identity and Access Management (IAM) and Cloud Key Management Services (KMS). Some of the results are quality dataset, documentation, visualization, and logs of monitoring after performing the tasks. The project allows UCW to examine trends, check for compliance and to improve on recruitment options through accurate, expandable and automated systems.

**Project Title:** Data Wrangling for Recruitment Data Analytics Using AWS

**Objective**
The purpose of this project is to clean, restructure, and consolidate the Recruitment Dataset into an organized, analytic format. AWS products including Amazon S3, EC2, AWS Glue, AWS Glue DataBrew, Athena, and DynamoDB are used in the project to guarantee data protection, accuracy, and preparedness for reporting and insights creation. 

**Background** Referral programs, candidate management, application processing, and confidentially storage are all steps in UCW's hiring process. Effective analysis of hiring patterns and compliance is hampered by duplication, incomplete fields, and discrepancies. AWS cloud-based solutions are used in this project to organize and safeguard hiring data in order to make better decisions. 

**Dataset**
1. Referral Program: Position types and incentives for referrals.
2. Application Selection Process: Submission Methods for Various Application Types. 
3. Candidate Management: Procedures for keeping track of candidate alerts, data, and notes. 
4. Confidentiality Storage: Guidelines for the retention and storage of different hiring papers. 
5. Blackout Period: Prohibitions on employment inside designated periods. 


**Methodology**

**Data Collection**
•Upload recruitment datasets to Amazon S3 as raw files for secure storage.
•Use Amazon EC2 instances to extract and prepare data from Excel files.

**Data Evaluation**

 Use AWS Glue for data profiling to identify missing values in fields like Referral Reward or Storage Period. 
-Duplicates in Candidate Management entries. 
- Inconsistent formatting for categorical variables, such as Hiring Type and Submission Method. 

**Data Cleaning:**

The following cleaning procedures will be automated by AWS Glue DataBrew: 
-Replace missing values (e.g., referral rewards) or remove incomplete rows. 
-Eliminate redundant entries in the procedures for candidate data. 
-Formats for categorical variables, including hiring type (administrative/faculty, for example), should be standardized. 
-Standardize the formats of dates for retention policies and blackout periods. 

**Data Transformation**
 In order to convert raw data into a format that can be used, AWS Glue will: 

-Convert date strings into datetime objects for trend analysis based on time.
- Analyzing referral rewards by position type to find critical trends. 
-The development of derived insights like "Documents Retention Compliance" or "Total Rewards Per Job Type." 

**Data Consolidation:**

Use DynamoDB to store the cleansed data in a single, unified dataset for organized, quicker access. 
• To extract insights from the dataset, use AWS Athena. For example, you can query the total referral incentives by position type. 
Adherence to the hiring blackout period. 
o The quantity of candidate notes destroyed or kept on file each year. 

**Monitoring and Validation:**
•	ETL performance will be tracked by AWS CloudWatch, which will also identify cleaning pipeline issues.
•	 All transformations and access will be recorded by AWS CloudTrail for traceability. 
•	 Data consistency and completeness will be guaranteed by using Athena for validation queries.

**Governance and Security:**

Use IAM roles and policies to manage who has access to private applicant information. 
Candidate notes and Referral Rewards are examples of fields that should be encrypted using AWS KMS (Key Management Service). 

**Technologies and Tools**

**Amazon S3:** A centralized location to store both raw and processed data. 

**Amazon EC2:** Processing power for preparing and extracting data. 

**AWS Glue:** An automated ETL tool for transformation, cleaning, and profiling. 

**AWS Glue Databrew:** AWS Glue DataBrew provides a visual interface for cleaning and normalizing datasets. 

**DynamoDB:** An organized database for aggregated hiring information. 

**AWS Athena:** A query tool for confirming the accuracy of data and producing new insights. 

**AWS CloudWatch and CloudTrail:** keeping an eye on things, recording them, and making sure the system is compliant. 

**IAM & KMS:** Encrypting sensitive data and controlling access to it. 

**Deliverables**
**Clean and Transformed Dataset:**
A professional, well-organized hiring dataset kept in DynamoDB. 
CSV files are exportable and can be used for reporting and sharing. 

**Comprehensive Report:**
Detailed description of the AWS tools used, cleaning, and transformation. 
Athena query-generated insights, such as hiring blackout compliance or referral reward patterns. 

**Monitoring Logs:**
To guarantee data integrity and traceability, use AWS CloudWatch and CloudTrail logs. 

**Timeline**

The project will be finished in 6 weeks.
**Weeks 1-2:** AWS Glue data ingestion, profiling, and evaluation. 
**Week 3–4:** Using AWS Glue DataBrew for cleaning and transformation. 
**Week 5:** Using Athena for validation and consolidating data into DynamoDB. 
**Week 6:** Documentation, reporting, and visualization. 

In order to provide UCW with meaningful insights on hiring practices, candidate management procedures, and referral programs, this project will provide a clean, organized, and secure recruitment dataset. Utilizing AWS solutions promotes better decision-making and compliance while guaranteeing scalability, automation, and data integrity. 

![image](https://github.com/user-attachments/assets/f17ebfa5-3017-4846-beb4-533abe5f3be9)


**Data Quality Measure for Recruitment Selection at UCW**

**Project Description**
The purpose of this project is to use AWS services to provide a Data Quality Control (DQC) framework for the University Canada West recruitment dataset. The framework supports efficient hiring procedures and decision-making by guaranteeing data accuracy, completeness, consistency, and dependability. AWS products for data profiling, cleaning, validation, enrichment, and monitoring will be used, including S3, Glue, DataBrew, Athena, DynamoDB, CloudWatch, and CloudTrail. The project resolves problems such as inconsistent formats, duplication, and missing values, guaranteeing safe storage, real-time monitoring, and reporting. Furthermore, for long-term gains, stakeholder training will encourage a culture of data governance and quality control.

**Project Title:** Implementing Quality Control Measures for Recruitment Data with AWS.

**Background:**The recruitment and selection dataset is critical for guaranteeing efficient recruiting, adherence to corporate policies, and data-driven decisions. The dataset's usability is compromised by issues like inconsistent formats, duplicate entries, and missing fields. The goal of this project is to employ AWS services to make sure that the hiring data is accurate, consistent, and prepared for use in effective hiring procedures.


**Scope:**
1. Data Profiling:  
   - Assessing completeness, correctness, and consistency of the dataset.

2. Data Cleaning:  
   - Removing duplicates and addressing missing values or inconsistent formats.

3. Data Validation:  
   - Implementing rules to enforce data correctness and format compliance.

4. Data Monitoring:  
   - Creating real-time dashboards and alerts for data quality tracking.

5. Data Protection:  
   - Encrypting and securing the dataset.

6. Training:  
   - Educating stakeholders on data quality management and AWS tools.

**Methodology:**

**Phase I (Week 1): Ingestion and Storage of Data**
-The recruitment dataset should be uploaded to Amazon S3 for centralized storage.
-To preserve historical records of modifications, enable S3 versioning. 
-To ensure safe access, configure IAM roles. 

***Phase II: Data Profiling (Week 2)**
- Create a catalog and examine the dataset using *AWS Glue Crawler*. 
-Utilize *AWS Glue DataBrew* to: - Determine which fields are lacking (such as Candidate Name and Application Date). 
-Analyze duplicates (such as email or candidate ID). 
-Emphasize formats that don't match, like the date formats in Application Date. 

**Phase III: Cleaning the Data (Weeks 3–4)**
- Use *AWS Glue DataBrew* to remove duplicate rows based on candidate ID or email. 
-"Not Applicable" is a default value that is used to replace missing data in fields such as Referral Reward. 
-Standardizing date formats (for example, application date should be YYYY-MM-DD). 
- Making categorical fields normal (e.g., capitalizing Land_Use_Label values).

**Phase IV: Validation of Data (Week 5)**
-Establish validation guidelines with *AWS Glue*:
-Make sure there are no duplicate candidate IDs. 
-The Referral Reward's numerical ranges should be checked. 
-Verify the application type by comparing it to an authorized list. 
-To guarantee compliance, query the dataset on Amazon S3 using *Athena*. 

**Phase V (Week 6): Enriching and Protecting Data**
-The cleansed dataset should be imported into *Amazon DynamoDB* using: 
-The Candidate ID is the main key. 
-Characteristics: Date of Application, Name of Candidate, Type of Position, and Referral Bonus. 

Enable *IAM-controlled access* and use *AWS KMS encryption* for security. 

**Phase VI: Week 7: Monitoring and Reporting**
-Make *CloudWatch* active to keep an eye on S3 and Glue tasks. 
-Use *CloudTrail* to record API communications. 
-Create dashboards for duplicate records using *CloudWatch* or *Athena* queries. 
- Missing values. 
- Compliance rates with the format. 

***Phase VII Training and Awareness (Week 8)* **
Create training sessions for HR departments to: - Explain the principles of data quality. 
- Display AWS tools and workflows. 
- Provide rules for reliable data entry. 

**Tools and technologies:**

*Amazon S3*: Used for raw and sanitized data storage. 
*AWS Glue/DataBrew*: For validation, cleansing, and profiling. 
*Amazon Athena*: For queries involving SQL. 
*Amazon DynamoDB*: For querying and structured access. 
*Amazon CloudWatch*: For monitoring in real time. 
*AWS CloudTrail*: For recording API activities. 
*IAM & KMS*: For encryption and safe access. 

***Deliverables*:**

1. *Cleaned Dataset*:  
   - Stored in S3 and DynamoDB for structured access.  

2. *Data Quality Metrics Report*:  
   - Includes completeness, correctness, and duplication rates.

3. *Monitoring Dashboard*:  
   - Real-time visualizations of data quality trends.

4. *Process Documentation*:  
   - Detailed methodologies and tools used.

5. *Training Materials*:  
   - For HR staff to ensure consistent practices.

**Timeline:**
The recruiting dataset at *University Canada West* will undergo a structured implementation of the *Data Quality Control (DQC)* project over *eight weeks* to guarantee thorough improvements in data quality. 

*In Week 1, the recruitment dataset will be transferred to **Amazon S3** for centralized storage. Secure access will be set up with *IAM roles*, and versioning will be enabled to track changes for future auditing.


*Week 2* focuses on *data profiling* with *AWS Glue Crawler* and *DataBrew* to analyze completeness, identify missing values, find duplicates, and highlight inconsistencies in areas such as Candidate ID, Referral Reward, and Application Date. 

**Glue DataBrew** will be used to clean data during *Weeks 3 and 4. Duplicate entries will be eliminated, missing values will be replaced with defaults, and formats that are inconsistent, such as dates, will be standardized. After cleaning, S3 will be used to store the dataset. 

In *Week 5, **Glue* and *Athena* will be used to construct validation rules. These guidelines verify that there are no duplicate Candidate IDs, check that numerical ranges are correct, and verify that the Application Type complies with authorized categories.


In *Week 6*, the emphasis is on *data enrichment* through the use of *DynamoDB* for structured searches and the implementation of security protocols like *KMS encryption* and IAM controls. 

During *Week 7,**CloudWatch* and *CloudTrail* will be utilized to log operations, monitor data pipeline performance, and display quality trends via dashboards. 

Finally, HR staff will participate in workshops and training sessions during *Week 8*, which will concentrate on uniform data input processes, AWS tools, and best practices for data quality.








