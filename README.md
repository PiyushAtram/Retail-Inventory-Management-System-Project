# Retail-Inventory-Management-System-Project

Overview 
 -This project is an end-to-end data pipeline that monitors product inventory and sends automated email alerts when stock levels are abnormal.

It helps identify:
  🔴 LOW STOCK (needs restocking)
  🟡 OVERSTOCK (excess inventory)

🛠️ Technologies Used
  -  Azure Data Factory 
  -  Azure Databricks (PySpark & SQL)
  -  Azure Logic Apps
  -  Delta Lake

⚙️ Workflow
  -  Data Ingestion
  -  Data is fetched and stored using Azure Data Factory
  -  Data Processing
  -  Data is cleaned and transformed in Databricks

Filtering Logic
  - Only important records are selected:
  - WHERE Status IN ('LOW STOCK', 'OVERSTOCK')

Integration
  Filtered data is sent from ADF to Logic App
  Notification
  Logic App processes the data and sends email alerts

💡 Key Features
  -  Automated pipeline from ingestion to alert
  -  Real-time stock monitoring
  -  Integration across multiple Azure services
  -  Handles JSON data between services

