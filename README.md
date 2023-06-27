This is a practice project on AWS for DE

argitecure diagram

![image](https://github.com/Chutchanan/AWS_DE_2/assets/134831110/f6927e6a-5a5f-4b98-835a-f701f9751de0)


brief procedure
- Upload all data to s3 using AWS CLI (see aws_cli.sh)
- Build glue crawler and catalog and query in Athena (to preview data and specify error on schema)
- convert csv to parquet and also change schema using Glue ETL (see pyspark.py)
- convert json to parquet using Lambda and also add trigger event to do job automatically. (see lambda.py)
- use crawler again to create clean data table from parquet file
- build ETL using glue ETL on top of 2 clean tables created to join for one analytic table and also add partition to optimize query cost for analysis job.
