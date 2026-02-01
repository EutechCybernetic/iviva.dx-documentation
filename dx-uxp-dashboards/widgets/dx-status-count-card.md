# DX Status Count Card

#### 1. Introduction

<figure><img src="../../.gitbook/assets/web and mobile (2) (1) (1).png" alt=""><figcaption></figcaption></figure>

The **DX Status Count Card** widget provides a quick visual overview of how many records fall into different categories within a DX application. It is commonly used to group and count transactions (such as work requests or issues) based on a selected field, such as **status**, **problem type**, or **priority**.

This widget helps users quickly identify **common issues**, **monitor activity**, and **spot trends** at a glance. It is available on both **web** and **mobile** **dashboards**, offering flexibility across devices.

***

#### 2. What Does It Show?

When added to a dashboard, the **DX Status Count Card** widget presents a compact layout that lists each **field value** (e.g., “Water leakage”, “Office Lights Flickering”) alongside its corresponding **transaction count**.

* Each card shows:
  * A label representing the group (e.g., type of issue)
  * A number representing how many transactions fall under that group
* The field used for grouping is fully configurable
* The display automatically updates based on the latest data

***

#### 3. Where Does the Data Come From?

This widget supports multiple data sources, but only **one** is used at a time, based on configuration:

* **iviva DX** – The default and most common option, pulling data directly from DX apps
* **API** – For external integration
* **iviva Service** – Uses backend services
* **Lucy** – Enables data to be retrieved from a low-code platform

> For this guide, we focus only on the i**viva DX** data source configuration, as other sources have been explained elsewhere.

***

#### 4. Data Source Component Breakdown (iviva DX)

<figure><img src="../../.gitbook/assets/1 (90).png" alt=""><figcaption><p>Configuration Popup</p></figcaption></figure>

When "iviva DX" is selected as the data source, the following fields appear for configuration:

**Component 1: DX Application**

Select the DX application from which the records should be counted (e.g., "Work Request").

**Component 2: Base Field**

Choose the field to group the data by. For example, you may select “Problem Title” to see a count of each problem type.

**Component 3: Base Options**

List the specific values (categories) from the base field that you want to track. Only these values will appear in the widget.

**Component 4: Filter Query (IQL)**

An optional field allows advanced filtering using an **iviva Query Language (IQL)** string. This allows you to limit the records displayed based on custom conditions.

***

#### 5. General Details Component Breakdown

This section controls how the widget is labeled on the dashboard.

**Component 5: Title**

Set a custom title for the widget (e.g., "Work Request Summary"). This title appears at the top of the widget and helps users quickly identify the context of the displayed data.

***

#### 6. Display Options

The **DX Status Count Card** widget adapts to your dashboard layout. It displays grouped data in a **vertical** or **grid** format depending on the available space.

* **Labels**: The field values appear as labels
* **Counts**: The counts appear as large numbers next to or below each label
* Display may vary slightly between **desktop** and **mobile** to ensure optimal readability

***

#### 7. Dashboard Visual Breakdown

This is how the widget appears after configuration:

<figure><img src="../../.gitbook/assets/1 (89).png" alt=""><figcaption></figcaption></figure>

**Component 1: Status Count Cards**

Each card represents a category based on the selected field and shows the number of records associated with it. This helps you quickly assess where the volume of activity is concentrated.

**Component 2: Grouped Field**

This field is used to group records. For example, if "Problem Title" is selected, each card represents a different problem category.

**Component 3: Transaction Count**

This is the number that shows how many records belong to each group. It provides insight into frequency or urgency at a glance.
