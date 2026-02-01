# DX All Transaction

#### 1. Introduction

<figure><img src="../../.gitbook/assets/web and mobile3 (1).png" alt=""><figcaption></figcaption></figure>

The **DX All Transaction** widget provides a comprehensive, scrollable view of all transactions within a specific DX application. It allows users to monitor, track, and explore both active and historical records —such as service requests, work orders, or issue logs—all in one place.

This widget is available on both **web** and **mobile dashboards**, offering a convenient way to stay on top of activities across devices.

***

#### 2. What Does It Show?

When added to the dashboard, the **DX All Transaction** widget presents a **list of transaction cards**. Each card provides a concise summary of an individual transaction, including key information such as:

* **Transaction ID**
* **Current status or stage**
* **Assignment information**
* **Priority Level**
* **Timestamps and Creator info**

A **filter icon** at the top of the widget allows users to select the specific application whose transactions should be displayed. This makes the widget dynamic and adaptable to multiple use cases.

***

#### 3. Where Does the Data Come From?

The widget supports data from the following sources:

* **iviva DX** – Pulls transactions directly from your DX apps
* **API** – Supports connection to external systems
* **iviva Service** – Uses backend service logic
* **Lucy** – Enables data to be retrieved from a low-code platform

> In this widget, **iviva DX is already configured internally**. Users do not need to manually set it during widget setup. \
> This guide focuses only on the **iviva DX data source configuration**, as other integrations are explained in separate sections.

***

#### 4. Data Source Component Breakdown (ivivaDX Only)

No custom configuration is required for the **iviva DX** data source in this widget. It comes **preconfigured**, and the DX application is selected through the **filter popup** during usage—not during the configuration stage.

> For this guide, we focus only on the i**viva DX** data source configuration, as others have been explained elsewhere.

***

#### 5. General Details Component Breakdown

This widget does not include a **General Details section**. The title and visual elements are **fixed** based on the widget’s purpose and layout.

***

#### 6. Display Options

The **DX All Transaction** widget is designed for **scrollable vertical viewing**. It adjusts based on different screen sizes. It supports:

* **Real-time transaction listing**
* **Dynamic filtering** by application
* **Responsive layout** for both desktop and mobile

The transaction cards are styled uniformly to present key details without clutter.

***

#### 7. Dashboard Visual Breakdown

<figure><img src="../../.gitbook/assets/1 (91).png" alt=""><figcaption></figcaption></figure>

Below is a component-wise explanation of the **DX All Transaction** widget appears on the dashboard:

**Component 1: Transaction List**

Displays all transactions associated with the DX app selected in the filter.

**Component 2: Filter Icon**

Located in the top-right corner of the widget. Clicking this icon opens the filter popup.

**Component 3: Application Selector**

A dropdown within the filter popup that lets users choose which DX app’s transactions to view.

**Component 4: Transaction Card**

Each card displays summary information for a transaction (ID, status, assignee, etc.). Clicking a card redirects the user to the detailed view of that transaction.

**Component 5: Transaction ID**

The unique identifier assigned to each transaction. This is useful for referencing and support.

**Component 6: Current Stage**

Indicates the transaction’s current progress (e.g., “NEW”, “In Progress”).

**Component 7: Assignment Info**

Shows who the transaction is assigned to, If no assignee exists, it displays “Unassigned”.

**Component 8: Metadata**

Includes creation date and time, priority (e.g., Medium, High), and the creator's name.
