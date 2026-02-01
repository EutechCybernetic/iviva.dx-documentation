# DX Rating

#### 1. Introduction

<figure><img src="../../.gitbook/assets/web and mobile (2) (5).png" alt=""><figcaption></figcaption></figure>

The **DX Rating** widget visually summarises how users have rated a particular transaction in a DX application. It displays key metrics like **average rating**, **star and face-based satisfaction levels**, and **the total number of ratings**. This provides a quick understanding of user satisfaction and helps track feedback over time.

Whether you are collecting feedback on individual transactions such as Work Requests, service visits, or issue resolutions, this widget presents a clear and interactive rating breakdown. It works seamlessly on both **web** and **mobile dashboards**.

***

#### 2. What Does It Show?

Once configured and placed on a dashboard, the widget displays:

* The **average rating** out of 5
* A visual breakdown of all ratings (1 to 5 stars)
* Percentage of users who selected each rating level
* Emojis or stars indicating satisfaction levels (based on settings)
* Total number of ratings collected

This makes it easy to monitor satisfaction trends related to individual transactions at a glance.

***

#### 3. Where Does the Data Come From?

This widget supports four data sources:

* **iviva DX** – Directly connects to DX apps (e.g., Work Request, Helpdesk)
* **API** – Connects to external rating sources
* **iviva Service** – Uses reusable backend services
* **Lucy** – Enables data to be retrieved from a low-code platform

> For this guide, we focus only on the **iviva DX** data source configuration, as others have been explained elsewhere.

***

#### 4. Data Source Component Breakdown (Iviva DX)

<figure><img src="../../.gitbook/assets/1 (97).png" alt=""><figcaption><p>Rating Widget Configuration</p></figcaption></figure>

When “iviva DX” is selected as the data source, the following fields become configurable:

**Component 1: DX Application**

Choose the DX application from which to pull rating data (e.g., “Work Request”).

**Component 2: Base Field**

Select the field that contains the actual rating values (e.g., “Ratings”).

**Component 3: Filter Query (IQL)**

(Optional) Enter advanced filtering logic if you want to narrow down the data to specific criteria (like a time range, user role, or status).

**Component 4: Enable Date Filter**

Toggle this ON if you want to limit ratings to a specific date range.

> When enabled, an additional field appears to select the **date field** used for filtering, such as “Created Date”.

***

#### 5. General Details Component Breakdown

This section allows you to fine-tune what’s shown in the widget:

**Component 5: Title**

Enter a custom title to display at the top of the widget (e.g., “Work Request Feedback Ratings”).

**Component 6: Show Total Count**

Enables the display of how many total ratings were collected across all selected transactions.

**Component 7: Show Average Rating**

Shows the average score calculated from all ratings.

**Component 8: Show Face Satisfaction**

Displays emoji faces (from happy to angry) to represent satisfaction levels based on rating.

**Component 9: Show Star Satisfaction**

Displays visual stars next to each rating row.

**Component 10: Show Rating Count**

Shows the raw number of ratings each star level received.

These toggles allow you to customise the widget based on your audience—whether you want a simple average or a full breakdown.

***

#### 6. Display Options

The widget adapts based on what you've chosen in the general settings:

* If **stars and faces** are both enabled, both visuals appear
* The rating breakdown bar shows **percentages** and **total counts**
* The layout automatically resizes and adjusts for mobile and desktop views
* The background and color theme are styled to match your dashboard

***

#### 7. Dashboard Visual Breakdown

<figure><img src="../../.gitbook/assets/1 (98) (1).png" alt=""><figcaption></figcaption></figure>

Here is what the widget looks like after configuration:

**Component 1: Average Rating**

At the top, the widget shows the overall average score out of 5, followed by visual stars.

**Component 2: Rating Breakdown Rows**

Each row represents a star level (from 1 to 5) and displays:

* An emoji face (if enabled)
* A percentage bar to show distribution
* A count of how many users selected that rating

**Component 3: Total Ratings Footer**

At the bottom, the widget shows the **total number of ratings** received across all levels.
