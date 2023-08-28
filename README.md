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

### What is Data Explorer and when is it a good fit?

Data Explorer is a fully managed, high-performance, big data analytics platform that makes it easy to analyze high volumes of data in near real time. The Azure Data Explorer toolbox gives you an end-to-end solution for data ingestion, query, visualization, and management.

By analyzing structured, semi-structured, and unstructured data across time series, and by using Machine Learning, Azure Data Explorer makes it simple to extract key insights, spot patterns and trends, and create forecasting models. Azure Data Explorer is scalable, secure, robust, and enterprise-ready, and is useful for log analytics, time series analytics, IoT, and general-purpose exploratory analytics.

**Note**: Data Explorer exists as both a Standalone offering (Azure Data Explorer) and part of Synapse (Synapse Data Explorer). All the content will apply to both these offerings (will be referred to as 'ADX') without any change.

ADX capabilities are extended by other services built on its powerful query language, including [Azure Monitor logs](https://docs.microsoft.com/en-us/azure/log-analytics/), [Application Insights](https://docs.microsoft.com/en-us/azure/application-insights/), [Time Series Insights](https://docs.microsoft.com/en-us/azure/time-series-insights/), and [Microsoft Defender for Endpoint](https://docs.microsoft.com/en-us/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint)


<img src="/assets/images/DX_Pic.png" width=800>


### Scenario 

Contoso is an enterprise services company that deals with data extraction, transformation, and load scenarios for it's customers who are using Azure native services like Azure Storage, Azure data factory, Azure SQL database.
Constoso also maintains audit traces,  system logs and telemetry from Azure services and data ETL processes. One customer recently approached Contoso asking to create a dashboard they can use to monitor their Azure SQL Database logs in a single place. Customer has agreed to provide a sample dataset to Contoso.

Contoso is planning to perform exploratory data analysis on the SQL DB logs. It is looking for a suitable analytics platform that provides out of the box integration with Azure services such as storage account for historical load and perform data analysis . Contoso is developing a SaaS application that will allow its customers to trace and monitor their system logs. Contoso wants to offer out of the box visualizations with interactive capabilities to enable its customers to drill-in/drill-out of the data and offer blazing fast loading of visualizations to its customers.

This workshop walks through the steps in designing, creating, and configuring Azure Data Explorer clusters keeping in mind these requirements. Once the cluster is deployed, this workshop enlists the steps to ingest data into ADX databases and tables using One Click ingestion.

### Pre-requisites
- Either a Microsoft account (MSA) or an Azure Active Directory (AAD) identity. This will be used to create free cluster.

### How to start with ADX
Generally, when starting with Azure Data Explorer, you will follow the following steps (ADX Workshop Labs will cover all these steps):
1. **Create a free ADX cluster**: To use Azure Data Explorer you first create a free cluster. An Azure Data Explorer cluster is the most basic unit.
2. **Create database**: Each cluster has one or more databases in that cluster. Each Azure Data Explorer cluster can hold up to 10,000 databases and each database up to 10,000 tables. 
3. **Ingest data**: Load data into database tables so that you can run queries against it. Azure Data Explorer supports several ingestion methods.
4. **Query data**: Azure Data Explorer uses the Kusto Query Language, which is an expressive, intuitive, and highly productive query language. It offers a smooth transition from simple one-liners to complex data processing scripts, and supports querying structured, semi-structured, and unstructured (text search) data. Use the web application to run, review, and share queries and results. You can also send queries programmatically (using an SDK) or to a REST API endpoint. 
5. **Visualize results**: Use different visual displays of your data in the native Azure Data Explorer Dashboards. You can also display your results using connectors to some of the leading visualization services, such as Power BI and Grafana. 

### Ready to go? Click on the below links to start the challenges
- [**Lab 1: Cluster Creation, Data Ingestion and Exploration**](https://github.com/Azure/ADX-in-a-Day-Lab1)

- [**Lab 2: Advanced KQL, Policies, and Visualization**](https://github.com/Azure/ADX-in-a-Day-Lab2)

