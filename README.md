# Power Bi

Introduction

Small and large businesses alike use data to make decisions about sales, hiring, goals and all areas for which they have data. While most businesses have access to data of one type or another, it can be intimidating for your average business user to understand the data without a background in data analytics or statistics. 

Power Bi takes intimidation and hassle out of data analysis and visualization. By connecting to one or more of the hundreds of existing data sources through a secure and simple interface, you can quickly and interact with and understand your data to influence all business systems.

In this module, we will:

  1. Describe the business value and features of Power Bi.

  2. Compare and contrast the different components that make up Power Bi.

  3. Describe how to clean and transform data.

  4. Examine how AI insights help detect anomalies and spot trends.

  5. Build a basic dashboard.

  6. Consume Power Bi reports and dashboards.

# Describe using power Bi to build data-driven analytics

From customer and employee data metrics for company goals, to sales and acquisitions, businesses are drowning in data, but this data is good as your ability to interpret and communicate its meaning.

Microsoft Power Bi is a collection of software services, apps and connectors that work together to turn your unrelated sources of data into coherent, visually immersive and interactive insights. Power Bi lets you connect to your data sources, clean, and model your data without affecting the underlying source, visualize what's important and share with anyone and everyone.

Power Bi consists of a Microsoft Windows Desktop application called Power Bi, an online SaaS service called Power Bi service and mobile Power Bi apps that are available on phones or tablet.

# Explore different Power Bi elements

To create Power Bi solutions, there are several major building blocks. These elements help not only what data is being presented, but also how it appears to those users who are consuming it. Those elements are datasets, dashboards and reports. All elements are organized into workspaces and they're created on capacities.

**Capacities**

Capacities are a core Power Bi concept that represents a set of resources used to host and deliver Power Bi content. They are either *shared* or *dedicated*. 

A *shared* capacity is shared with other Microsoft customers.

A *dedicated* capacity is fully committed to a single customer. Dedicated capacities require a subscription. By default, shared workspaces are created on a shared capacity.

**Workspaces**

- These are containers for dashboards, reports, datasets and dataflows in Power BI. There are 2 types of workspaces: my workspace & workspaces.

  * My workspace - is the personal workspace for any Power BI customer to work with your own content. Only you have access to your My workspace. You can share dashboards and reports or create an app, then you want to work in a workspace.
 
  * Workspaces - are used to collaborate and share content with colleagues. You can add colleagues to your workspaces and collaborate on dashboards, reports and datasets. With one exception, all workspace members need Power BI Pro licenses.
 
  ![image](https://github.com/MisterWest11/Power-Bi/assets/152319557/6b83f745-770f-4beb-85e6-0adb7699e073)

Workspaces are also the places where you create, publish and manage apps for your organization. Think of workspaces as containers and staging areas for the content that makes up a Power BI app.

An appp is a collection of dashboards and reports built to deliver key metrics to the Power BI consumers in your organization. Apps are interactive, but consumers can't edit them.

**Semantics Models**

A semantic model in Power Bi is like a big container that holds data you import or connect to from various sources. The data can come from Excel files, other Power BI models or even cloud services like Salesforce. These models are linked to workspaces, so anyone with access to the workspace can see the data in the model, as long as they have the right permissions.

They are associated with workspaces and a single semantic model can be part of multiple workspaces. When you open workspace, the associated semantic models are listed under semantic models. Each listed item semantic model represents a collection of data. 

Centralized Data Hub: A semantic model acts like a central storage for data you import or connect to in Power BI.

Variety of Sources: It can bring together data from various sources like Excel files, cloud services (e.g., Salesforce), and even other Power BI models.

Dataflows: Dataflows can also be a source for semantic models. (Dataflows are likely methods to prepare and manage data before feeding it into the model).

Workspace Connection: Semantic models are linked to specific workspaces in Power BI.
Shared Access: Any member of a workspace with admin, member, or contributor permissions can see the data in the associated semantic model.

Reusable Model: A single semantic model can be part of multiple workspaces, promoting data reusability.

In simpler terms, a semantic model helps you gather data from different places into one container within a workspace, making it easy for authorized users to access and analyze the combined data.

**Shared semantic models**

Collaboration is Key: BI thrives on teamwork. Sharing well-defined semantic models fosters collaboration.

Standardized Models = One Source of Truth: Consistent models ensure everyone uses the same data definitions, leading to reliable reports and a single source of truth for decision-making.

Reuse and Efficiency: Pre-built, optimized models save time for report creators, allowing them to focus on analysis and insights.

Healthy Data Culture: Shared models promote data accessibility and understanding, fostering a data-driven culture within your organization.

Consuming Shared Models: Power BI makes it easy to utilize these shared semantic models when building reports.

In essence, standardized semantic models act as a foundation for consistent, collaborative, and efficient BI practices in your organization.

# Describe cleaning and transforming data in Power BI Desktop

Data from different sources often requires cleaning and transformation: Data from various systems might not be compatible or structured for combined analysis.

Example scenario: Building a device usage report requires customer details (CRM) and IoT data (Azure IoT Hub).

Power BI Desktop as a tool for data transformation: This application helps you prepare the data for visualization.

You've also introduced the three main views in Power BI Desktop:

Report view: For building visualizations and arranging them for presentations.

Data view: Shows the data structure, allowing for measure creation, new columns, and relationship management.

Model view: Provides a visual representation of data model relationships, enabling management and modification.

Data transformation: Making data usable for reports by removing columns, duplicating them, or replacing values.

Clean data for better visualizations: Power BI prefers columnar data, and cleaning helps transform messy formats (like spreadsheets with multi-span headers) into a more suitable structure.

Power Query tools for data preparation: This built-in toolset helps you clean and format data before using it in reports.

The provided reference seems like a valuable resource for further learning on data transformation in Power BI: "Transform, shape, and model data in Power BI".

# Describe using AI Insights to spots trends and anomalies

Power BI's insights feature helps organizations easily identify insights such as anomalies and trends in your data as you interact and consume elements such as reports, dashboards and visualizations.

![image](https://github.com/MisterWest11/Power-Bi/assets/152319557/4c76f559-b979-43af-a9ba-80eb8116505c)

Power BI has multiple insights features that use AI:

  * Insights for reports: Analyze data and finds anomalies and trends in your data as you interact with reports.

  * Insights for individual visuals: Analyzes and explains the fluctuations of data points in visuals.

  * Insights for dashboard tiles: Looks at the data being used to render that tile and presents them in interactive visuals.

  * Quick insights for datasets: Automatically generate data insights on a datasets in the Power BI services.

  * AI insights for data models in Power Query: Provide access to pretrained machine learning models from Azure Cognitive Services.


*Notifications*

They are an important part of the insights capabilities in Power BI. When Power BI identifies insights, presented with a notification. Notifications are a great way to proactively interact with suggested insights to ensure that you're not missing anything important such as sales in a specific region increased. 

**Get insights on reports and visuals**

Types of Insights:

Anomalies: Identify unexpected data points that deviate significantly from the expected range. 

These can be helpful for investigating potential issues or outliers.

Subtypes: Significant anomaly, Recent anomaly, Anomaly summary.

Explanations: Power BI suggests possible reasons for the anomaly by analyzing related dimensions in your data model.

Trends: Detect patterns of increase or decrease over time in your data. Power BI removes noise and seasonality to focus on meaningful trends.

Subtypes: Long trend, Steep trend, Recent trend, Trend reversal.

Explanations: Power BI identifies categories that most significantly influence the trend.

KPI Analysis: Evaluates how a current value compares to a defined target (if available) or to other data segments (if no target is set).

Target vs No Target: Analysis considers variance from the target or the absolute value itself.

Explanations: Power BI highlights categories with higher or lower than expected values. Ranking is based on Z-scores for target vs non-target scenarios.

Overall, these insights in Power BI can be valuable tools for uncovering hidden patterns, identifying potential problems, and gaining a deeper understanding of your data.
