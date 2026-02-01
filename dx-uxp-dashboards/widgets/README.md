# Widgets

In UXP, **widgets** are pre-built, configurable components that enable users to create dynamic, interactive dashboards **without writing any code**. These widgets serve as the building blocks of your dashboard and can be used to:

* Visualize data
* Display summaries
* Present charts
* Manage content
* Interact with various system modules across both web and mobile environments

Each widget is designed with a specific purpose—whether it is rendering charts, showing transaction summaries, mapping asset locations, or displaying SLA performance—making it easy to build powerful dashboards tailored to your use case.

**UXP widgets are**:

* **No-code**: Easily configurable through the platform's UI.
* **Reusable**: Applicable across multiple dashboards or applications.
* **Responsive**: Optimized to work seamlessly on both web and mobile interfaces.
* **Dynamic**: Widgets can be data-driven, fetching real-time or scheduled data updates from your configured sources.

***

### How to Use Widgets to Build Dashboards

Creating a dashboard in **UXP** using widgets involves **selecting**, **configuring**, and **arranging** the desired widgets according to your business requirements. Below is a typical workflow:

1. **Choose Your Widgets**\
   Select from the wide range of available UXP widgets (e.g., **DX Pie Chart**, **DX Summary Card**, **DX My Apps**). Each widget serves a specific function—some are designed to display KPIs, others to show charts or maps.
2. **Configure Widget Properties**\
   Each widget includes a configuration panel where you can:
   * Define the **data source** or **query** it uses.
   * Customise **field mappings**, **titles**, and **thresholds**.
   * Enable behaviors such as a redirection, coloring rules, drill-downs, etc.
3. **Drag and Drop into the Layout**\
   Use the **layout editor** to position widgets on your dashboard. Arrange them in rows, columns, or grid structures to reflect your reporting or operational requirements.
4. **Iterate and Enhance**\
   UXP widgets are flexible—update configurations anytime based on evolving data sources or user needs evolve, **all without writing any code**.

***

### Widget Categories (Examples)

* **Visual Analytics**: \
  DX Line Chart, DX Pie Chart, DX Bar Chart, DX SLA Comparison Chart
* **Summary Views**: \
  DX Summary Card, DX Tile Card, DX Object Count, DX Asset Summary Count
* **Navigation and Content**: \
  DX My Apps, DX Portfolio Sidebar, DX NewsFeed
* **Geospatial Widgets**: \
  DX Map View, DX Location Layout Map View
* **Custom Interaction**: \
  DX Number Field, DX Rating, DX Web View

***

With UXP widgets, anyone—from analysts to non-technical stakeholders—can build professional dashboards in minutes, enabling faster decision-making and delivering clear, actionable insights without requiring any development expertise.



### Common Widget Configuration Sections

Each UXP widget is designed to be **fully configurable** through a user-friendly interface. Regardless of the widget type, you will typically encounter the following **core configuration sections**:

<figure><img src="../../.gitbook/assets/image (124).png" alt=""><figcaption></figcaption></figure>

In a widget, clicking the **settings icon** opens the configuration popup **when the dashboard is in edit mode**. If the widget has not yet been configured and the dashboard is in **view mode**, a message is displayed with a **"Configure"** button, which also launches the configuration popup.

***

### 1. Data Source

The **Data Source** section specifies where the widget retrieves its data. It forms the foundation for how the widget displays meaningful and accurate information.

<figure><img src="../../.gitbook/assets/1 (86).png" alt=""><figcaption><p>Different data sources available</p></figcaption></figure>

**Data source types supported**:

* **iviva DX**
* **API**
* **iviva Service**
* **LUCY**

***

#### 1.1. iviva DX

The i**viva DX** option is used when a widget retrieves data directly from existing iviva DX applications. such as **Work Request**, **Incident Management**, **Assets**, **Service Desk**, and more.

When selected, you can:

* Choose a **DX Application** as the data source.
* Configure the **Base Field** that determines which data is displayed or grouped in the widget.
* Optionally define **Base Options** and apply **filter queries (IQL)** to control the dataset shown.

> **Note**:\
> The exact configuration fields and how data is interpreted will vary between widgets. These details are explained separately within each individual widget’s documentation.

This option is the most commonly used source when you want your widget to reflect **live data directly from operational modules** within the iviva.DX ecosystem.

***

#### 1.2. API

#### API Integration

Widgets that support **API** as a data source allow you to connect to external systems using configurable HTTP requests. This method is ideal when your data resides outside iviva DX and needs to be pulled dynamically.

<figure><img src="../../.gitbook/assets/1 (83).png" alt=""><figcaption></figcaption></figure>

\
Here’s a breakdown of each component in the API configuration panel:

***

**API Configuration Panel Components**

**Component 1: HTTP Method**

* Select the type of request to make:
  * **`GET`** – Fetch data without modifying server-side resources.
  * **`POST`** – Submit data and receivie a response (e.g., filtered results).

***

**Component 2: End Point**

* Enter the full URL of the API to connect to.
* This is where the widget will send the request.
* **Example**:\
  `https://otbapps.dx.servicedeskhq.com/API/Locations`

***

**Component 3: Header Parameters**

* Optional headers that may be required by the API (e.g., `Authorization`, `Content-Type`, etc.).
* These are passed with the HTTP request to handle:
  * Authentication
  * Data formatting
  * Caching control

***

**Component 4: Query Parameters**

Define the parameters to send with the request. Each parameter includes:

* **Type**
* **Name**
* **Optional value source**

***

#### Parameter Configuration

_This setup applies to both **Header Parameters** and **Query Parameters** in the configuration panel._

**Component 5: Supported Parameter Types**

This defines **where the parameter value is sourced from**:

* **Query String** – The widget fetches values directly from the query string portion of the URL.&#x20;
  * Example:  if the URL is `...?key=123`, and if the parameter name is `key`, the value `123` is used.
* **Static** – A fixed value manually entered by the user. This value remains constant unless edited in the config.
* **Environment** – The value is derived from environment variables such as current user details, tenant, or session-specific context.
* **List** – The value is dynamically retrieved from a selected list item or record currently in context (e.g., `LocationKey` selected in another widget).

***

**Component 6: Parameter Name / Field**

This field behaves differently depending on the selected **Parameter Type**:

* For **Query String** or **Static**, you must manually enter the **exact key** that the endpoint expects (e.g., `userkey`, `type`, `max`).
* For **Environment** or **List**, you can select from the available fields provided by the system or the list context (e.g., `TenantID`, `LocationKey`, `Assignee`).

***

**Important Note on Endpoint and Parameter Matching**

Ensure that the **parameter name** you configure **matches exactly the parameter name expected by the API service.**

**If the names do not match**, the parameter will not resolve correctly, and the iviva service may receive incorrect or incomplete data.

***

**Component 7: IsRequired**

A checkbox that marks the parameter as **mandatory**. If enabled, the widget will not function unless a valid value is supplied for this parameter.

***

**Component 8: Value From**

This defines **how** the parameter obtains its value:

* For **Static** – Manually type the fixed value.
* For **List** or **Environment** – Select a value from available fields.
* For **Query String** – Automatically extracts the value from the current page URL.

***

**Component 9: Expected Response**

This section shows a **sample API response** (usually in JSON format) expected by the widget.\
This helps you:

* Understand the data structure.&#x20;
* Identify the fields available for binding or charting.

***

#### 1.3. iviva Service

Widgets that support **iviva Service** as a data source can retrieve information through **system-level service** **models** defined within the **iviva DX platform**. This allows you to pull structured data from backend services without relying on external APIs.

<figure><img src="../../.gitbook/assets/1 (84).png" alt=""><figcaption></figcaption></figure>

\
**Configuration Overview**\
Below is a breakdown of each component in the **iviva Service Configuration Panel**:

***

**Component 1: App Name**\
Select the **iviva DX** application from which the service is defined (e.g., Asset Management, Work Request, etc.).\
This selection filters the available **models** and **services** relevant to that specific app.

***

**Component 2: Use Custom Service**\
Toggle this **ON** to manually define a service instead of selecting from predefined options.\
When enabled, you can type the service name manually rather than selecting it from the dropdown (e.g., Model: Service). \
This is useful when integrating with **custom or dynamic service logic** that is not listed by default.

***

**Component 3: Model Name**\
Choose the **data model** within the selected app that the widget should use (e.g., `LocationModel`, `AssetModel`).\
Models define the **schema** and **structure** for both the service request and the expected response.

***

**Component 4: Service Name**\
Select the available **service operation** to invoke (e.g., `GetLocations`, `FetchAssets`).\
This determines the logic executed and the response returned to the widget.

***

**Component 5: Parameters**\
This section allows you to define any **additional inputs** required by the selected service (e.g., filters or dynamic limits).\
Similar to API integration, parameters are defined using several supporting fields:

***

#### Parameter Configuration

**Component 6: Supported Parameter Types**

This defines **where the parameter value is sourced from**:

* **Query String** – The widget fetches values directly from the query string portion of the URL. For example, if the URL is `...?key=123`, and the parameter name is `key`, the value `123` is used.
* **Static** – A fixed value manually entered by the user. This never changes unless edited in the config.
* **Environment** – The value is derived from environment variables such as current user details, tenant, or session-specific context.
* **List** – The value is dynamically retrieved from a selected list item or record currently in context (e.g., `LocationKey` selected in another widget).

***

**Component 7: Parameter Name / Field**

This field behaves differently based on the selected parameter type:

* If the type is **Query String** or **Static**, you must manually type in the **exact key** the endpoint expects (e.g., `userkey`, `type`, `max`).
* If the type is **Environment** or **List**, you’ll be prompted to choose from available fields provided by the system or the list context (e.g., `TenantID`, `LocationKey`, `Assignee`).

***

**Important Note on Iviva Service and Parameter Matching**

You must ensure that **the name you configure matches the parameter name that the iviva service is expecting**

**If the names don’t match**, the parameter will not resolve properly, and the iviva service will receive incorrect or missing data.

***

**Component 8: IsRequired**

A checkbox that marks the parameter as **mandatory**. If enabled, the widget will not work unless a valid value is provided for this parameter.

***

**Component 9: Value From**

This defines how the parameter gets its value:

* For **Static** – Manually type the fixed value.
* For **List** or **Environment** –Select from available fields.
* For **Query String** – The value is extracted from the current page URL.

***

**Component 10: Expected Response**\
This section shows a sample response format (usually JSON) that the service is expected to return.\
It helps you understand how to map this data inside the widget for visual output.

***

#### 1.4. Lucy&#x20;

**Lucy** is a **low-code platform** within iviva DX that enables users to configure intelligent models, define logic, and optionally write custom code. Widgets that support **Lucy** as a data source can leverage these models to power dashboards with  rule-based decisions or custom responses.

This integration is ideal for bringing intelligence and automation into your dashboard components—without the need to build full-fledged services or APIs.

<figure><img src="../../.gitbook/assets/1 (85).png" alt=""><figcaption></figcaption></figure>

Below is a breakdown of each component in the **Lucy configuration panel**:

***

**Component 1: Lucy Model**\
Select the logic model created within the **Lucy** platform (e.g., `RiskAssessmentModel`, `ServiceRoutingModel`).\
These models are built through a low-code interface, allowing users to configure logic visually and if required, embed custom scripts.

***

**Component 2: Lucy Action**\
Choose a specific **action** defined within the selected **Lucy** model (e.g., `GetSummary`, `PredictOutcome`).\
Actions determine the type of operation or evaluation the model will execute when triggered by the widget.

***

**Component 3: Parameters**\
Define the input parameters to be passed to the **Lucy** model at runtime.\
These parameters influence the model's behavior and control the scope or filters of its response.

Configuration is similar to other integrations, using the following components:

***

**Component 4: Supported Parameter Types**

This defines where the parameter value is sourced from:

* **Query String** – The widget fetches values directly from the query string portion of the URL. For example, if the URL is `...?key=123`, and the parameter name is `key`, the value `123` is used.
* **Static** – A fixed value manually entered by the user. This never changes unless edited in the config.
* **Environment** – The value is derived from environment variables such as current user details, tenant, or session-specific context.
* **List** – The value is dynamically retrieved from a selected list item or record currently in context (e.g., `LocationKey` selected in another widget).

***

**Component 5: Parameter Name / Field**

This field behaves differently based on the selected parameter type:

* If the type is **Query String** or **Static**, you must manually type in the **exact key** the endpoint expects (e.g., `userkey`, `type`, `max`).
* If the type is **Environment** or **List**, you’ll be prompted to choose from available fields provided by the system or the list context (e.g., `TenantID`, `LocationKey`, `Assignee`).

***

**Important Note on Lucy and Parameter Matching**

You must ensure that **the name you configure matches the parameter name that the lucy service is expecting**

**If the names don’t match**, the parameter will not resolve properly, and the iviva service will receive incorrect or missing data.

***

**Component 6: IsRequired**

A checkbox that marks the parameter as **mandatory**. If enabled, the widget will not work unless a valid value is provided for this parameter.

***

**Component 7: Value From**

This defines how the parameter gets its value:

* For **Static** – You manually type the fixed value.
* For **List** or **Environment** – You select from available fields.
* For **Query String** – The value is extracted from the current page URL.

***

This integration allows widgets to interact directly with Lucy’s low-code intelligence engine—bringing automation, data transformation, and predictive capability right into the user interface.

***

### 2. General Details

This section defines how the widget appears visually and what it represents to the end user.

This ensures that each widget is not only informative but also matches the look and feel of your overall dashboard theme.

***

### 3. Import/Export Configuration

This section helps manage widget configurations across different dashboards or environments without recreating settings from scratch.

* **Export**: Download the current widget configuration as a JSON file.
* **Import**: Upload a previously exported configuration to quickly reuse settings.

This feature is especially useful for:

* Replicating widget setups between **staging** and **production** environments.
* Sharing configuration templates across **teams**.
* Backing up **complex configurations** for future use.
