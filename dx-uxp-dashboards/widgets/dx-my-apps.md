# DX My Apps

1\. **Introduction**

<figure><img src="../../.gitbook/assets/web and mobile (1).png" alt=""><figcaption></figcaption></figure>

The **DX My Apps** widget is a personalised launcher that displays the list of applications available to you within the UXP dashboard. Acting like a smart app menu, It provides **quick access** to the tools and systems you regularly use, such as **Work Requests**, **Helpdesk**, **Cleaning Schedules**, or **Energy Management**.

This widget works seamlessly on both **web** and **mobile dashboards**, ensuring a consistent experience no matter what device you use.

***

#### 2. What Does It Show?

When added to a dashboard, the **My Apps** widget presents a series of **app cards**. Each card typically displays:

* **App Name**
* **App Icon**
* **Short Description**&#x20;

Each card is **clickable** and redirects the user to the **Create Transaction** page of that particular application.

***

#### 3. Where Does the App List Come From?

The list of apps you see is automatically loaded based on your **account access**. These apps may originate from different sources depending on how the dashboard is configured, such as:

* **iviva DX Apps** – Applications built into the iviva DX ecosystem.

<figure><img src="../../.gitbook/assets/1 (96).png" alt=""><figcaption></figcaption></figure>

Below is a breakdown of the data source section visible in the configuration popup:

***

**Component 1: App List Display Area**\
This section displays the **currently selected applications** that appear in the widget. Each row represents one DX application.

* Apps like "Work Request", "Service Request", "Work Permit", etc., are listed here.
* You can click the **trash icon** next to any item to remove that app from the list.

***

**Component 2: DX Application Dropdown**\
This dropdown allows you to **select a new application** from the Iviva DX platform to add to the list.\
Only the apps that exist and are available in the system will appear here.

***

**Component 3: Horizontal Layout Toggle**\
This toggle controls the layout of the application display.\
When turned on, the selected applications are shown horizontally inside the widget.

***

**Component 4: Add Button**

After selecting an app, click this button to add it to the list of summary cards.

This configuration lets you control exactly which apps are displayed in the widget, giving flexibility based on the user’s role or operational focus.

{% hint style="info" %}
Only this data source is available for this widget.
{% endhint %}

***

#### 4. Display Options

The way apps appear on your screen may vary depending on how your dashboard was designed:

* **Horizontal or Vertical View** – Apps can either scroll **left-to-right** or be stacked **top-to-bottom**.

<figure><img src="../../.gitbook/assets/1 (93) (1).png" alt=""><figcaption></figcaption></figure>

**Component 1:** The **DX My Apps** widget displays the list of applications configured for the user. Each card represents an app that can be accessed for performing specific tasks or workflows.

**Component 2:** Each card represents a specific application. When you hover over a card, a **plus icon** (+) appears. Clicking the **plus icon** redirects the user to the **Create Transaction** page of that particular application.
