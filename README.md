# Covid19 Prediction and Reporting Pipeline


## Solution Architecture
![image](https://github.com/pratik3848/Covid19-Prediction-and-Reporting/assets/41427089/c166f32e-e284-414d-9ece-bc07a09f9d33)

## Data Sources
- ### European Centre for Disease Prevention and Control (ECDC)
- ### Eurostat Website

## Storage Solutions
- ### Azure Blob storage (population data)
- ### Azure Data Lake Gen2 (processed data)
- ### MySQL DB (reporting)

## Transformation Tools
- ### Azure Data Flow (simple transformation and code free)
- ### Databrics (PySpark and SparkSQL)

## Parameters Flow within Pipeline
- ### Trigger -> Pipeline -> Dataset(maps the data pulled from linked service, for source and sink) -> Linked Service (forms a connection to the source and sink)

## Triggers Used
- ### Event Based Trigger
- ### Schedule Trigger

## Data Orchestration
- ### Ingest and Process Population Data using Parent Pipeline based on Event Based Trigger
- ### Ingest and Process ECDC Data using Dependency based Tumbling Window Trigger

## Pipeline Monitoring
- ### Azure Data Factory Monitor (pipeline and trigger failure alerts for the last 45 day runs)
- ### Azure Monitor (store the logs for analysis)

## Continuous Integration/Continuous Delivery (CI/CD)
 - ### Azure DevOps

## Data Visualization
### PowerBI

## Final Reports
![image](https://github.com/pratik3848/Covid19-Prediction-and-Reporting/assets/41427089/18b10671-c1b8-43ba-b8a3-0f61132966b6)
![image](https://github.com/pratik3848/Covid19-Prediction-and-Reporting/assets/41427089/d35fa1f7-ff47-4523-b61d-e59bd6c2007c)
![image](https://github.com/pratik3848/Covid19-Prediction-and-Reporting/assets/41427089/763d0df9-6273-4e98-9e4e-dbdcdbd8fa67)

