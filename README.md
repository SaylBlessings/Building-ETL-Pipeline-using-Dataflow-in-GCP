# Building-ETL-Pipeline-using-Dataflow-in-GCP

## Overview

This project showcases a cloud-native data warehousing solution by integrating Google Cloud Storage (GCS) with BigQuery using Cloud Functions, enabling efficient data management and analysis. To begin, access permissions are configured by creating a service account with the necessary roles, including Storage Object Viewer for GCS access and BigQuery Data Editor for BigQuery access. Next, a Cloud Function trigger is set up to automate data ingestion, specifying the GCS bucket and event type (Finalize/Create) to execute the function when new data is uploaded. The Cloud Function itself is written in Python or Node.js, extracting data from GCS, transforming it using libraries like Pandas and NumPy, and loading it into BigQuery using the BigQuery client library. The function creates a BigQuery dataset and table, loads the transformed data, and handles errors and exceptions using try-except blocks. Logging and monitoring are also implemented using Stackdriver Logging and Monitoring. By integrating these GCP services, the project enables seamless data extraction, transformation, and loading, facilitating efficient data analysis and management. It utilizes the following GCP services:

- Google Cloud Storage (GCS)
- Cloud Functions
- BigQuery
- Dataflow
- Stackdriver Logging and Monitoring

## Architecture

The following diagram illustrates the project architecture:

GCS -> Cloud Function -> Dataflow -> BigQuery

## Prerequisites

To run this project, you need:

- A GCP account
- A GCS bucket
- A BigQuery dataset and table
- A Cloud Function with the necessary permissions
- Dataflow API enabled

## Setup and Configuration

To set up the project, follow these steps:

1. Create a service account with the necessary roles.
2. Set up a Cloud Function trigger to automate data ingestion.
3. Write a Cloud Function in Python or Node.js to extract data from GCS, transform it, and load it into BigQuery.
4. Configure Dataflow pipeline to read data from GCS, transform it, and load it into BigQuery.

 
## Running the Pipeline

To run the pipeline, follow these steps:

1. Upload data to GCS.
2. Trigger the Cloud Function.
3. Run the Dataflow pipeline.

## Monitoring and Logging

The pipeline uses Stackdriver Logging and Monitoring to log and monitor the pipeline's execution.

## Conclusion

This project demonstrates a cloud-native data warehousing solution using GCP services. The pipeline enables efficient data management and analysis by automating data ingestion, transformation, and loading.

 
## Contributing

Contributions are welcome! Please submit a pull request with your changes.
