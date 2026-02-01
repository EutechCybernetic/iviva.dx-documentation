# DX Tile Card

#### **1. Introduction**

<figure><img src="../../.gitbook/assets/web and mobile (2).png" alt=""><figcaption></figcaption></figure>

The **DX Tile Card** widget is a compact visual that displays the count of specific items from your chosen application. It is ideal for highlighting key metrics such as total work requests, issue counts, or any other trackable field, giving users a quick, high-level overview.

***

#### **2. What Does It Show?**

This widget shows the **total count** of records that match your configured criteria. You can select the field to count by, specify values to include, and optionally set up a link that opens another page or application when the tile is clicked.

***

#### **3. Where Does the Data Come From?**

The **DX Tile Card** supports four types of data sources:

* **iviva DX** – Default and most common option, pulling data directly from DX apps
* **API** – For external integration
* **iviva Service** – Uses backend services
* **Lucy** – Enables data to be retrieved from a low-code platform

> For this guide, we focus only on the i**viva DX** data source configuration, as others have been explained elsewhere.

***

#### **4. Data Source Component Breakdown (ivivaDX)**

<figure><img src="../../.gitbook/assets/1 - 2025-06-07T090032.985.png" alt=""><figcaption></figcaption></figure>

**Component 1 – DX Application**\
Selects the iviva application (like “Work Request”) from which the tile pulls its data.

**Component 2 – Base Field**\
Determines which field's values are counted. For example, “Problem Title” may list issues like “Water leak” or “Flickering lights.”

**Component 3 – Base Options**\
Lets you choose which specific field values you want to include in the count. The tile will only consider these values when calculating the total.

**Component 4 – Filter Query (IQL)**\
An optional advanced filter where you can define custom conditions to narrow down the data shown.

***

#### **5. General Details Component Breakdown**

<figure><img src="../../.gitbook/assets/1 - 2025-06-07T090548.285.png" alt=""><figcaption></figcaption></figure>

**Component 1 – Title**\
Specifies the heading that appears on the tile. This is usually the name of the field or category being counted (e.g., “Problem Title”).

**Component 2 – Enable Search Link**\
When turned on, clicking the tile will redirect users to the app’s built-in search page (based on the same filters).

{% hint style="info" %}
_Note: This option cannot be used if "Enable Link" is turned on._
{% endhint %}

**Component 3 – Enable Link**\
Lets you activate a custom URL that opens when users click the tile. Useful for linking to other apps or dashboards.

{% hint style="info" %}
_Note: This option cannot be used if "Enable Search Link" is turned on._
{% endhint %}

**Component 4 – Custom Link URL**\
This is the actual web address (e.g., `https://youtube.com`) the tile will open if the custom link is enabled.

**Component 5 – Add Parameters**\
You can add URL parameters if you need to pass specific data in the custom link, such as a record ID or user key (Parameter configuration explained in detail below).

**Component 6 – Visual Customization (White Mode, Background & Text Color)**\
Allows you to personalise the look of the tile. Choose white mode or define custom background and text colors to match your dashboard theme.

***

**Parameter Configuration**&#x20;

**Supported Parameter Types:**

| Parameter Type | Description                                                                             |
| -------------- | --------------------------------------------------------------------------------------- |
| `Query String` | Appended to the API URL as `?key=value`. Common in GET requests.                        |
| `Static`       | Manually define a fixed value.                                                          |
| `Environment`  | Value is pulled dynamically from environment-specific settings.                         |
| `List`         | Used when you want to pass multiple values for a single parameter (e.g., `?ids=1,2,3`). |

* Parameter Name/Field:&#x20;
  * This input changes its behavior based on the selected **Parameter Type**:
    * If the **Parameter Type** is `Query String` or `Static`, you must manually provide the **exact key** expected by the API or service (e.g., `max`, `type`).
    * If the **Parameter Type** is `Environment` or `List`, a **Field** must be selected from the available data context (e.g., environment-bound variables or list-type fields).
* IsRequired: Checkbox to mark if the parameter must always be included.
* Value From: Define how the value is derived—either typed manually or selected from the context.

***

#### **6. Display Options**

* **Title Display**: The entered title is shown clearly on the tile.
* **Record Count**: The main focus of the tile is the large number that represents the count.
* **Link Behavior**: If enabled, clicking the tile opens a search page or a custom link.
* **Visual Styling**: Customizable text and background color for enhanced dashboard design consistency.

***

#### **7. Dashboard Visual Breakdown**

<figure><img src="../../.gitbook/assets/1 - 2025-06-07T091259.531.png" alt=""><figcaption></figcaption></figure>

**Component 1 – Interaction**\
If a link (search or custom) is enabled, clicking the icon on the top right will open the linked page in a new tab.

**Component 2 – Count Display**\
The center of the tile shows the count of matching entries (e.g., how many times “Water leak” occurred).

**Component 3 – Title**\
The tile displays the user-defined title at the middle (e.g., “Problem Title”).

**Component 4 – Styling**\
If configured, the tile may appear in white mode or show a custom background and text color.
