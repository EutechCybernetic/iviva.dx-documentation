# DX Object Count

#### **1. Introduction**

<figure><img src="../../.gitbook/assets/web and mobile1.png" alt=""><figcaption></figcaption></figure>

The **DX Object Count** widget is designed to show the total number of records for a specific object, such as assets or users. This widget provides a quick and focused numerical snapshot in a compact tile format, making it perfect for high-level monitoring dashboards.

***

#### **2. What Does It Show?**

This widget displays:

* A single number indicating the total count of records from the chosen object (e.g., 6 assets).
* A title to describe what the count represents.
* An icon that visually represents the selected object (e.g., asset icon for "Asset Count").

***

#### **3. Where Does the Data Come From?**

The widget supports data from the following sources:

* **iviva DX** – Default and most common option, pulling data directly from DX apps
* **API** – For external integration
* **iviva Service** – Uses backend services
* **Lucy** – Enables data to be retrieved from a low-code platform

> For this guide, we focus only on the i**viva DX** data source configuration, as others have been explained elsewhere.

***

#### **4. Data Source Component Breakdown (IvivaDX only)**

<figure><img src="../../.gitbook/assets/1 - 2025-06-07T092659.256.png" alt=""><figcaption></figcaption></figure>

**Component 1: Choose an Object**\
Select the main object you want to count, such as Asset, User, or Work Request.

**Component 2: Static Filters**\
Allows you to apply specific filters to refine the data—for example, filtering by a specific asset type or department.

**Component 3: Filter Options**\
Choose specific values under the selected filter type to limit the count (e.g., only assets from a particular building). Filter types include Asset, Installed Location, Asset Category, and Site. Based on the selected filter type, you can then choose a specific filter value.

**Component 4: Landscape View**\
Enable this option to switch the tile’s layout from a vertical view to a wider horizontal layout.

***

#### **5. General Details Component Breakdown**

<figure><img src="../../.gitbook/assets/1 - 2025-06-07T092942.261.png" alt=""><figcaption></figcaption></figure>

**Component 1: Title**\
This is the text shown below the number in the tile (e.g., “Asset Count”), helping users understand what is being counted.

**Component 2: Background Color**\
Set the background color of the tile to match the theme of your dashboard.

***

#### **6. Display Options**

* **Tile Orientation**: Optionally toggle to a landscape layout.
* **Theme Customization**: Modify the background color for better visual appeal.
* **Icon & Layout**: The icon shown is based on the selected object (e.g., assets, users).

***

#### **7. Dashboard Visual Breakdown**

<figure><img src="../../.gitbook/assets/1 - 2025-06-07T093102.344.png" alt=""><figcaption></figcaption></figure>

**Component 1: Icon**\
A relevant icon (e.g., cube for assets) is displayed at the top of the tile.

**Component 2: Count**\
The main number (e.g., 6) is prominently displayed in the center.

**Component 3: Title**\
Displayed underneath the number, this title reflects the selected label (e.g., “Asset Count”).

**Component 4: Background Color**\
The entire tile adopts the color defined in the configuration, improving visual organization.

***
