# Event-Driven Data Pipeline integrating Cloud Pub/Sub with On-Premise SQL Server

![NRDB_to_Mssql_flowchart - Copy](https://github.com/Omi-sudo/pub_sub_to_SQL_server/assets/82666181/b59edfb2-0034-48d8-9dce-1e7b7e01eb70)

Architecture Diagram:  Event-Driven Data Pipeline integrating Cloud Pub/Sub with On-Premise SQL Server at Transunion.

🌟 Project Highlights:

# Event-Driven Architecture:

Messages published in a Pub/Sub topic trigger Cloud Functions, initiating the data pipeline workflow.

# Data Processing and Transformation:

Cloud Functions read Parquet files from GCS buckets in a separate project.
Execute transformation logic on the data, processing it into a structured format.
Data Landing in GCS:

Processed data is landed into our project's GCS bucket in CSV format.

# Composer Pipeline Activation:

A secondary Cloud Function is triggered upon data landing, initiating a Cloud Composer pipeline.

# Chunked Data Processing:

Composer pipeline processes CSV data in chunks, optimizing resource utilization and scalability.
Data Storage in MS SQL Server:

Processed data is stored in real-time in our on-premise MS SQL Server, ensuring seamless integration.

# Key Responsibilities:

Collaborated with cross-functional teams to design and implement the event-driven architecture.
Utilized Google Cloud services (Pub/Sub, Cloud Storage, Cloud Functions) for efficient data movement.
Orchestrated data processing and transformation using Cloud Composer.
Ensured seamless integration with an on-premise MS SQL Server for real-time data storage.

# Technology Stack:

Google Cloud Pub/Sub,
Cloud Storage,
Cloud Functions,
Cloud Composer and
MS SQL Server
