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
