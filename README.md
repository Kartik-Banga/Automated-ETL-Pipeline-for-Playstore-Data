**Automated-ETL-Pipeline-for-Playstore-Data**

I recently concluded an end-to-end data pipeline project that seamlessly utilizes AWS services with Power BI for comprehensive analytics. 
Focused on Play Store data, the project comprised distinct phases, demonstrating a well-orchestrated data flow. 

1) Data Cleaning with AWS Lambda:
   Initiated by employing AWS Lambda functions and Python scripts (utilizing Pandas and NumPy) for comprehensive data cleaning of the 'playstore_review' dataset.
   This approach ensured meticulous attention to data quality and integrity. The refined dataset was then securely stored in an S3 bucket,
   laying the foundation for subsequent stages of the pipeline.
2) Metadata Extraction with AWS Glue Crawlers:
   Leveraged AWS Glue Crawlers to extract essential metadata from the cleaned review dataset,
   establishing a structured foundation for the pipeline.
3) ETL with PySpark in AWS Glue Job:
   Orchestrated a PySpark script within an AWS Glue Job, seamlessly integrating SQL queries through 'spark.sql,' along with Spark functions,
   to execute an inner join between 'playstore_apps' and the cleaned 'playstore_review' datasets. This multifaceted approach not only facilitated dataset
   merging but also enabled the application of advanced SQL-based data cleaning techniques, resulting in a thoroughly polished dataset.
5) Automated Workflow with AWS Step Functions:
   Implemented AWS Step Functions for seamless orchestration, automating the entire data pipeline.
   This streamlined execution of Lambda functions, Glue jobs, and other processes, ensuring a coherent end-to-end workflow.
6) Storage and Accessibility on S3:
   * **The decision not to use Amazon Redshift** was primarily driven by cost considerations. Given the scale and scope of the project, leveraging Amazon S3 for
     storage proved to be a more cost-effective solution, aligning with budget constraints while still meeting analytical requirements.*
   
   Stored the final, cleaned, and merged dataset in an S3 bucket in CSV format, establishing a scalable and accessible storage solution. 

7) Power BI Analysis for Actionable Insights:
   Utilized Power BI for in-depth analysis, creating visually compelling dashboards and reports.
   This phase provided actionable insights into Play Store apps, enhancing decision-making capabilities.




