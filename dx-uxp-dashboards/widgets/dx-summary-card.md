# DX Summary Card

#### 1. Introduction

<figure><img src="../../.gitbook/assets/web and mobile (4).png" alt=""><figcaption></figcaption></figure>

The **DX Summary Card** widget provides users with a quick, high-level overview of the current state of transactions across multiple DX applications. It helps visualise workload distribution by summarizing how many transactions are **Open**, **Assigned**, or **Closed** within each selected application.

Ideal for **operational monitoring**, this widget enables users to **track activity across various applications in a single view**, making it easier to manage priorities and maintain awareness of application-specific progress.

This widget is available on both **web and mobile dashboards**.

***

#### 2. What Does It Show?

When added to a dashboard, the **DX Summary Card** widget displays a series of **summary blocks**, one for each configured application. \
\
Each block shows:

* The **name of the application**
* A count of transactions under the following statuses:
  * **Open**
  * **Assigned**
  * **Closed**

These statuses reflect the current stage of each transaction, making it easy to spot bottlenecks or activity spikes.

***

#### 3. Where Does the Data Come From?

The **DX Summary Card** widget supports the following data sources:

* **iviva DX** – The default and most common option, pulling data directly from DX apps.
* **API** – For integrating with external sources
* **Service** – Uses backend services
* **Lucy** – Enables low-code/AI-based processing

> For this guide, we focus only on the **iviva DX** data source configuration, as others have been explained elsewhere.

***

#### 4. Data Source Component Breakdown (iviva DX)

<figure><img src="../../.gitbook/assets/1 (94) (1).png" alt=""><figcaption></figcaption></figure>

\
When i**viva DX** is selected as the data source, the widget allows you to select and display summaries from multiple DX applications.

\
**Component 1: Configured Application List**

This section displays the list of applications currently added to the widget. Each app appears as a separate summary card in the final dashboard view. You can remove any app using the trash icon.

\
**Component 2: DX Application Dropdown**

Use this dropdown to select a new DX application from the system. Once selected, the application will appear in the list above and be displayed in the dashboard summary.

\
**Component 3: Add Button**

After selecting an application, click this button to add it to the list of summary cards.

This configuration gives you full control over which apps appear in the widget, giving flexibility based on the user roles or operational focus.

***

#### 5. General Details Component Breakdown

> ⚠️ **Note**: This widget does not include a **General Details** sectio&#x6E;**.** The layout and titles are automatically managed based on the selected applications.

***

#### 6. Display Options

The **DX Summary Card** widget is designed with a clean vertical layout, that stacks each application's summary card one after the other.

* Each card is styled with the app’s **icon** and **color.**
* The layout is **responsive,** automatically adjusting to different screen sizes.
* Suitable for both **detailed dashboards** and **compact summary views**.

***

#### 7. Dashboard Visual Breakdown

<figure><img src="../../.gitbook/assets/1 (95).png" alt=""><figcaption></figcaption></figure>

Here’s how the **DX Summary Card** widget appears on the dashboard, broken into its main components:



**Component 1: DX Summary Card Widget**\
Represents the widget as a whole. It displays all the apps added in the configuration, each with its corresponding set of transaction status counts.\
\
**Component 2: Individual Application Card**\
Each card corresponds to a single DX application (e.g., Work Permit, Issue Inventory). All transaction stages for that app are grouped under this card.\
\
**Component 3: Application Name**\
The title at the top of each card indicates you which DX app the summary belongs to.\
\
**Component 4: Transaction Stages**\
Shows the stage categories (e.g., Open, Assigned, Closed) allowing users to understand what phase transactions are in.\
\
**Component 5: Transaction Counts**\
Next to each stage, the widget displays the **number of transactions** currently in that state. This helps prioritize actions and monitor workflow progress.

***
