# Azure Data Explorer in a Day (Preview)

Synapse Customer Success Enginnering team is pleased to present this ADX-in-a-day learning experience. The Hands on workshop is a challenge based, discover by doing experience divided into 2 parts of 4 Hours each, a total of 8 hours. 

- [**Lab 1: Cluster creation and data ingestion**](https://github.com/Azure/ADX-in-a-Day-Lab1)
This Lab will focus on enabling the participants to design ADX based big data analytics solution, create an ADX cluster, and ingest data into the cluster - One click ingestion of historic data and update policy to perform ETL.
// To Do: Explore historical load using one clik ingestion(Already available). Transformation function using .set-or-append, Materialized Views, Functions, Update policy, . Complete end-to-end data load scenario can be covered


- [**Lab 2: Data exploration and visualization using Kusto Query Language (KQL)**](https://github.com/Azure/ADX-in-a-Day-Lab2)
This Lab will focus on enabling the participants to write Kusto queries to explore and analyze the data stored in the clusters. Participants will also create cool visualizations. It is recommended to complete the Lab 1 before beginning with Lab 2.

---
Earn a digital badge! In order to receive the ADX-in-Day completion digital badge, you will need to complete the challenges marked with 🎓 in each Lab. Please submit the KQL queries/commands using the answer sheet found at the beginning of Lab. </br></br>
---
<p align="center"><img src="/assets/images/badge.png" width="200"></p>


### What is Data Explorer and when is it a good fit?

Data Explorer is a fully managed, high-performance, big data analytics platform that makes it easy to analyze high volumes of data in near real time. The Azure Data Explorer toolbox gives you an end-to-end solution for data ingestion, query, visualization, and management.

By analyzing structured, semi-structured, and unstructured data across time series, and by using Machine Learning, Azure Data Explorer makes it simple to extract key insights, spot patterns and trends, and create forecasting models. Azure Data Explorer is scalable, secure, robust, and enterprise-ready, and is useful for log analytics, time series analytics, IoT, and general-purpose exploratory analytics.

**Note**: Data Explorer exists as both a Standalone offering (Azure Data Explorer) and part of Synapse (Synapse Data Explorer). All the content will apply to both these offerings (will be referred to as 'ADX') without any change.

Data Explorer capabilities are extended by other services built on its powerful query language, including [Azure Monitor logs](https://docs.microsoft.com/en-us/azure/log-analytics/), [Application Insights](https://docs.microsoft.com/en-us/azure/application-insights/), [Time Series Insights](https://docs.microsoft.com/en-us/azure/time-series-insights/), and [Microsoft Defender for Endpoint](https://docs.microsoft.com/en-us/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint)

### Scenario 

Contoso is a supply chain logistics company that runs a fleet of ships, trucks, and cargo planes to transport and deliver goods around the world. Some of the world’s largest enterprises rely on Contoso’s logistics capabilities to deliver goods to their end customers. Contoso has invested in connecting its fleet with sensors that measure temperature, pressure, humidity, tilt, shock, and light exposure inside its fleet. These sensors emit telemetry data every 1 minute, property data whenever there is a change in the device property, and command data whenever a new command is executed. 

Contoso is looking for suitable analytical solution that provides out of the box integration with Azure services such as storage account for historical load and perform data analysis . Contoso is developing a SaaS application that will allow its customers to track, trace and monitor their shipments. Contoso wants to offer out of the box visualizations with interactive capabilities to enable its customers to drill-in/drill-out of the data. Contoso will offer its customers to view and analyze the last 6 months data. Contoso will retain every customer’s data for up to 1 year. Contoso wants to offer blazing fast loading of visualizations to its customers.
This workshop walks through the steps in designing, creating, and configuring Azure Data Explorer clusters keeping in mind these requirements. Once the cluster is deployed, this workshop enlists the steps to ingest data into ADX databases and tables using various integration methods such as One Click ingestion.

### Pre-requisites
- An Azure subscription
- Upload the files in Data\Logistics_telemetry_Historical in to a storage account container
- Authorization to create an Azure Data Explorer cluster or Synapse Data Explorer Pool

### How to start with ADX
Generally, when starting with Azure Data Explorer, you will follow the following steps (ADX Workshop Labs will cover all these steps):
1. **Create an ADX cluster**: To use Azure Data Explorer you first create a cluster. An Azure Data Explorer cluster is the most basic unit.
2. **Create database**: Each cluster has one or more databases in that cluster. Each Azure Data Explorer cluster can hold up to 10,000 databases and each database up to 10,000 tables. 
3. **Ingest data**: Load data into database tables so that you can run queries against it. Azure Data Explorer supports several ingestion methods.
4. **Query data**: Azure Data Explorer uses the Kusto Query Language, which is an expressive, intuitive, and highly productive query language. It offers a smooth transition from simple one-liners to complex data processing scripts, and supports querying structured, semi-structured, and unstructured (text search) data. Use the web application to run, review, and share queries and results. You can also send queries programmatically (using an SDK) or to a REST API endpoint. 
5. **Visualize results**: Use different visual displays of your data in the native Azure Data Explorer Dashboards. You can also display your results using connectors to some of the leading visualization services, such as Power BI and Grafana. 

### Ready to go? It's Lab time!
- [**Lab 1: Cluster creation and data ingestion**](https://github.com/Azure/ADX-in-a-Day-Lab1)

 // To Do: Include challenges from Microhack -

 // Challenge 1: Create an ADX cluster

 // Challenge 3: Starting with the basics of KQL

 // Challenge 4: Explore and transform data
 
 // Challenge 7: Materialized views, Functions, External Tables

- [**Lab 2: Data exploration and visualization using Kusto Query Language (KQL)**](https://github.com/Azure/ADX-in-a-Day-Lab2)

- // To Do: Include challenges from Microhack -
- // Challenge 8: Caching and retention policies
- // Challenge 9: Control commands
- // Challenge 5: Advanced KQL operators
- // Challenge 6: Visualisation

