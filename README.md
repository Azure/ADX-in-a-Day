# Microsoft Fabric Real-Time Analytics in a Day

Welcome to a One Day, Hands on workshop on Microsoft Fabric Real-Time Analytics. Microsoft Customer Success team is delighted to present this challenge based, discover by doing experience divided into 2 labs of 4 Hours each, a total of 8 hours.


## After the workshop, you'll better understand how to
- Create KQL database in your Fabric enabled Power BI workspace
- Ingest data into KQL database
- Run Powerful KQL queries to explore the data
- Manage KQL database using control commands and policies
- Visualize data in KQL database Dashboards


 [**Lab 1: Database Creation, Data Ingestion and Exploration**](https://github.com/Azure/ADX-in-a-Day-Lab1)
This Lab will focus on enabling the participants to Create a KQL database, and ingest data into the KQL database table - One click ingestion of historic data , update policy to perform ETL and write some KQL queries. 

 [**Lab 2: Advanced KQL, Policies, and Visualization**](https://github.com/Azure/ADX-in-a-Day-Lab2)
This Lab will focus on enabling the participants to write Kusto queries to explore and analyze the data stored in the KQL database. Participants will also create cool visualizations. It is recommended to complete the Lab 1 before beginning with Lab 2.

---
Earn a digital badge! In order to receive the Microsoft Fabric Real-Time Analytics in a Day completion digital badge, you will need to complete the challenges marked with ✅ in each Lab. Please submit the results using the answer sheet found at the beginning of Lab. </br>

<p align="center"><img src="/assets/images/badge.png" width="300"></p>

---

### What is KQL Database and when is it a good fit?

Microsoft Fabric Real-Time Analytics is a fully managed, high-performance, big data analytics platform that makes it easy to analyze high volumes of data in near real time. The Microsoft Fabric Real-Time Analytics toolbox gives you an end-to-end solution for data ingestion, query, visualization, and management.

By analyzing structured, semi-structured, and unstructured data across time series, and by using Machine Learning, Microsoft Fabric Real-Time Analytics makes it simple to extract key insights, spot patterns and trends, and create forecasting models. Microsoft Fabric Real-Time Analytics is scalable, secure, robust, and enterprise-ready, and is useful for log analytics, time series analytics, IoT, and general-purpose exploratory analytics.

**Note**: KQL Databse exists as both a Standalone offering (Azure Data Explorer) and part of Microsoft Fabric (KQL Databse). The content will apply to KQL Databse offering in Microsoft Fabric. More about differences between Real-Time Analytics and Azure Data Explorer here: https://learn.microsoft.com/en-us/fabric/real-time-analytics/realtime-analytics-compare

KQL Databse capabilities are extended by other services built on its powerful query language, including [Azure Monitor logs](https://docs.microsoft.com/en-us/azure/log-analytics/), [Application Insights](https://docs.microsoft.com/en-us/azure/application-insights/), [Time Series Insights](https://docs.microsoft.com/en-us/azure/time-series-insights/), and [Microsoft Defender for Endpoint](https://docs.microsoft.com/en-us/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint)


<img src="/assets/images/DX_Pic.png" width=800>


### Scenario 

Contoso is an enterprise services company that deals with data extraction, transformation, and load scenarios for it's customers who are using Azure native services like Azure Storage, Azure data factory, Azure SQL database.
Constoso also maintains audit traces,  system logs and telemetry from Azure services and data ETL processes. One customer recently approached Contoso asking to create a dashboard they can use to monitor their Azure SQL Database logs in a single place. Customer has agreed to provide a sample dataset to Contoso.

Contoso is planning to perform exploratory data analysis on the SQL DB logs. It is looking for a suitable analytics platform that provides out of the box integration with Azure services such as storage account for historical load and perform data analysis . Contoso is developing a SaaS application that will allow its customers to trace and monitor their system logs. Contoso wants to offer out of the box visualizations with interactive capabilities to enable its customers to drill-in/drill-out of the data and offer blazing fast loading of visualizations to its customers.

This workshop walks through the steps in designing, creating, and configuring Azure Data Explorer clusters keeping in mind these requirements. Once the cluster is deployed, this workshop enlists the steps to ingest data into ADX databases and tables using One Click ingestion.

### Pre-requisites
- Either a Microsoft account (MSA) or an Azure Active Directory (AAD) identity. This will be used to create free cluster.

### How to start with ADX
Generally, when starting with KQL Database in Fabric, you will follow the following steps (Fabric RTA Workshop Labs will cover all these steps):
1. **Create database**: Create KQL Database in Fabric Real-Time Analytics. 
2. **Ingest data**: Load data into database tables so that you can run queries against it. KQL Database supports several ingestion methods.
3. **Query data**: KQL Database uses the Kusto Query Language, which is an expressive, intuitive, and highly productive query language. It offers a smooth transition from simple one-liners to complex data processing scripts, and supports querying structured, semi-structured, and unstructured (text search) data. Use the web application to run, review, and share queries and results. You can also send queries programmatically (using an SDK) or to a REST API endpoint. 
4. **Visualize results**: Use different visual displays of your data in the native KQL Database Dashboards. You can also display your results using connectors to some of the leading visualization services, such as Power BI and Grafana. 

### Ready to go? Click on the below links to start the challenges
- [**Lab 1: Cluster Creation, Data Ingestion and Exploration**](https://github.com/Azure/ADX-in-a-Day-Lab1)

- [**Lab 2: Advanced KQL, Policies, and Visualization**](https://github.com/Azure/ADX-in-a-Day-Lab2)

