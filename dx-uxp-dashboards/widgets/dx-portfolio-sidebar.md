# DX Portfolio Sidebar

#### 1. Introduction

<figure><img src="../../.gitbook/assets/web and mobile2 (1).png" alt=""><figcaption></figcaption></figure>

The **DX Portfolio Sidebar** is a widget that provides a snapshot of facilities and quick navigation links to other dashboards. It is ideal for users who manage multiple facilities or assets and want fast access to key portfolio information—without leaving their current view.

***

#### 2. What Does It Show?

The widget visually presents:

* Total number of facilities
* Area statistics including total, common, and commercial space
* A list of individual facilities, each with quick access buttons
* A "Quick Access" section containing manually configured dashboard links for fast navigation

***

#### 3. Where Does the Data Come From?

{% hint style="info" %}
No external data source needs to be configured. The widget pulls internal facility information directly from the platform and allows manual linking to dashboards created in the system.
{% endhint %}

***

#### 4. Data Source Component Breakdown (iviva.DX only)

{% hint style="info" %}
Not applicable – this widget does not require iviva.DX or any other data source configuration.
{% endhint %}

***

#### 5. General Details Component Breakdown

{% hint style="info" %}
Not applicable – this widget does not include a General Details configuration section.
{% endhint %}

***

#### 6. Quick Access Dashboard Links Configuration

<figure><img src="../../.gitbook/assets/1 - 2025-06-08T232814.800.png" alt=""><figcaption></figcaption></figure>

This section lets you configure navigation links to dashboards grouped by a selected dashboard type.

**Component 1: Dashboard Type**

Use the **Dashboard Type** dropdown to choose the group of dashboards you want to manage:

* **Location**: For facility or location-based dashboards
* **Asset**: For dashboards related to specific assets\
  &#xNAN;_&#x54;he selected type determines which dashboard displayed in the widget._

***

**Component 2: Dashboard Links**

A list showing all links you have added. Each entry shows the link group (e.g., Location, Portfolio) and the linked dashboard title.\
Each row also includes a red delete icon (X) to remove the link.

***

**Component 3: Link Name**

Text field to enter the label that will be displayed in the widget under 'Quick Access'

***

**Component 4: Link Dashboard**

Dropdown menu that lists all dashboards available for linking. You select one to associate with the name given in Component 3.

***

**Component 5: Add Button**

Click this button to add the link defined in Component 3 and 4 into the Dashboard Links list. If any required fields are missing, validation messages will appear.

***

#### 7. Display Options

* **For Location Dashboard Type**:
  * A **toggle switch** appears at the top right of the widget.
    * Toggle to the left: Shows the Location **View** (facility count, area details, facility list)
    * Toggle to the right: Shows only the **Quick Access** dashboard links
* **For Asset Dashboard Type**:
  * The toggle is not shown.
  * Only the **Quick Access** view is shown by default.

***

#### 8. Dashboard Visual Breakdown

This section shows how the widget looks and behaves on the dashboard depending on the configuration.

#### Location Type

<figure><img src="../../.gitbook/assets/1 - 2025-06-08T233719.856.png" alt=""><figcaption></figcaption></figure>

**Component 1: Portfolio Sidebar Widget**

* Displays the title **“PORTFOLIO”**
* A toggle switch appears at the top right. When set to left, it shows detailed facility stats (like now).
* Shows the **total number of facilities** with a large circular badge (in this example, _5 Facilities)_.
* Below that, it displays total area in square meters, broken down into:
  * **Common Area**
  * **Commercial Area**
* This section gives a quick snapshot of the overall space distribution.

***

**Component 2: List of Facilities**

* Under the **FACILITIES** section, each item (like mda, Africa, colombo) represents an individual facility in the portfolio.
* For each facility, the name and area (e.g., _0 m²_) are displayed alongside a building icon.
* These act like shortcuts that allow users to quickly identify specific facilities

***

**Component 3: Action Icons**

* Located on the right side of each facility card:
  * **First icon** (arrow): Opens the configured dashboard for that link
  * **Second icon** (star): Pins the facility for prioritised visibility
* These icons enhance interactivity and allow users to customise their sidebar experience.

***

#### Asset Type

<figure><img src="../../.gitbook/assets/1 - 2025-06-08T234624.484.png" alt=""><figcaption></figcaption></figure>

**Component 1: Portfolio Sidebar Widget**

* Displays the section title '**QUICK ACCESS'**
* &#x20;When the Dashboard Type is **Location**, a toggle switch appears at the top-right.
  * When set to the **right**, it switches the sidebar to this **compact view**.
  * If Dashboard Type is **Asset**, this toggle does **not appear**—the widget always loads in this compact style.&#x20;

***

&#x20;**Component 2: Configured Link**

* Shows the **configured dashboard link**—**Location** in this example
* Clicking any of these will take you to the respective configured dashboard view.

***

**Component 3: Clear All**

* The **“CLEAR ALL”** button located on the right, allows you to do the following actions:
  * **Removes all items listed under LINKS**
  * **Unpins them** from the expanded sidebar (if user switches back to expanded mode).

{% hint style="info" %}
A section labeled '**LINK'** displays any **pinned items**.

* In this example, '**Kandy'** is pinned and shown with:
  * A location pin icon on the left
  * The facility name
  * A pin icon on the right, indicating it is actively pinned
* Clicking any of these pinned links also takes the user to the respective dashboard configured during setup.
{% endhint %}
