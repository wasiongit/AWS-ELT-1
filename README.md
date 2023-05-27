# Data Flow 
 1. Compressed Data in .zip format, uploaded to S3 bucket
 2. Data stored in an AWS S3 bucket
 3. Using Glue Crawler to get the schema and other table formation data, Glue stores that in AWSDataCatalog
 4. Transforming the data using Athena, Athena saves the query output data in a predefined S3 bucket
 5. Athena can be accessed over Python via API and so did in this case.
 6. I got the transformed output data in the S3 bucket.
 7. Data has been loaded to the Redshift data warehouse from the S3 bucket and now the data can be used for analytics or other ML tasks.
![Machine Leaning Gig (1)](https://github.com/wasiongit/AWS-ELT-1/assets/84765303/55685d76-7585-48a8-9b05-8d8887935d51)
