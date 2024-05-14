# Stock Market Data Analysis Using Kafka and AWS 

## Objective:
    To design and implement a robust data pipeline for real-time processing and analysis of stock market data using modern data processing technologies(Kafka) and cloud services.
## Technologies used:
    1. Programming Language : Python
    2. Database : SQL
    3. Apache Kafka
    4. Amazon Web Services (AWS) : EC2, S3, Glue, Crawlers, Athena

## Architecture:
![Architecture](https://github.com/pradhanmona7/Stock-Market-Data-Analysis-Using-Kafka-and-AWS/assets/114325852/5d8f89f8-1b3c-47c6-8b1d-42126ae6cb12)

## Steps:
### 1. Data Source:
        We began with a CSV file containing the raw data. CSV files are commonly used for data exchange and are easily readable by both humans and machines.
### 2. Data Transformation:
        Using Python, we converted the CSV data into JSON format. This conversion was necessary because real-time data often adheres to JSON standards, making it more compatible with modern data processing tools and technologies.
### 3. Data Processing with Kafka:
        We utilized Kafka as a message broker to handle the storage and processing of data. Kafka provides a distributed, fault-tolerant platform for real-time data streaming, enabling efficient data processing and management.
        Within Kafka, we set up both producers and consumers. Producers are responsible for publishing data to Kafka topics, while consumers retrieve and process the data from these topics.
        To ensure scalability and reliability, our Kafka cluster was hosted on an EC2 instance in AWS. This setup allowed us to handle large volumes of data and maintain high availability.
### 4. Data Storage with AWS S3:
        After processing the data through Kafka, we securely stored it in AWS S3. S3 is a highly scalable and durable object storage service provided by Amazon Web Services.
        Storing the data in S3 ensures that it is readily accessible, highly available, and can scale to accommodate growing data volumes.
### 5. Data Cataloging with AWS Glue:
        To facilitate efficient data management and analysis, we utilized AWS Glue to crawl and catalog the data stored in S3.
        AWS Glue automatically discovers and catalogs data, providing a structured schema that makes it easier to query and analyze the data.
### 6. Data Analysis with Athena:
        With the data cataloged by AWS Glue, we loaded it into Athena for analysis. Athena is a serverless, interactive query service that allows you to analyze data stored in S3 using standard SQL.
        Leveraging Athena's SQL-like query capabilities, we were able to perform robust data analysis to uncover insights into stock market trends and patterns

## References
    1. Video tutorial - [https://www.youtube.com/watch?v=KerNf0NANMo](https://www.youtube.com/watch?v=KerNf0NANMo)
    2. AWS Account Tutorial - https://www.youtube.com/watch?v=kbtDJHgjrPc
    3. Github project - https://github.com/darshilparmar/stock-market-kafka-data-engineering-project
  
