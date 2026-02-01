# DX Asset Summary Count

#### **1. Introduction**

<figure><img src="../../.gitbook/assets/web and mobile (9) (1).png" alt=""><figcaption></figcaption></figure>

The **Asset Summary Count** widget provides a clear, visual overview of your organisation's asset status. Displayed as colour-coded tiles, each segment represents a specific asset category, allowing users to quickly assess asset conditions such as active use, allocation, disposal, and warranty status.

***

#### **2. What Does It Show?**

This widget displays counts of assets categorised into four key groups:

* **Active Assets**: Assets currently in operational use
* **Disposed Assets**: Assets that have been discarded and are no longer active
* **Allocated Assets**: Assets that have been assigned to a specific user or department
* **Warranty Expired Assets**: Assets whose warranty periods have ended

Each category is shown in a tile with a distinct colour and icon, making it easy to distinguish different asset types at a glance.

***

#### **3. Where Does the Data Come From?**

This widget supports the following data sources:

* **API** – Pulls data from a configured external API
* **iviva Service** – Uses a backend service to retrieve custom data
* **Lucy** – Fetches data from a low-code platform

***

#### **4. Data Source Component Breakdown**

> **Note:** There is no configurable data source component for iviva.DX in this widget. The data is automatically retrieved from the built-in asset modules, so you do not need to set anything up. That said, you can still choose to pull data from other sources if needed.

***

#### **5. General Details Component Breakdown**

<figure><img src="../../.gitbook/assets/1 - 2025-06-09T153118.891.png" alt=""><figcaption></figcaption></figure>

**Component 1: Title**\
The Title field gives your widget a custom title—it will show up at the top of the dashboard. This helps set your widget apart from other summary widgets or adapt it to a specific use case—like '_Building A – Asset Overview'._

***

#### **6. Display Options**

* **Colour-coded Tiles**: Each asset category has a dedicated colour and icon for quick visual cues.
* **Grid Layout**: Tiles are laid out in a neat 2×2 grid for for balanced presentation and readability.
* **Counts Only**: The widget shows numeric values—no detailed records.
* **No Additional Filters**: This widget is designed for quick summaries—no filters or drill-downs here.

***

#### **7. Dashboard Visual Breakdown**

<figure><img src="../../.gitbook/assets/1 - 2025-06-09T153639.229.png" alt=""><figcaption></figcaption></figure>

**Component 1: Widget Title**

* The configured title shows up at the top of the widget.

**Component 2: Active Assets Tile**

* Shows how many assets are currently in use
* Has a barcode icon and a blue background

**Component 3: Disposed Assets Tile**

* Displays the count of assets that have been removed or discarded
* Uses a red background and a trash icon for clear visual contrast

**Component 4: Allocated Assets Tile**

* Indicates how many assets have been assigned to users or departments
* Uses an orange background with an allocation icon

**Component 5: Warranty Expired Assets Tile**

* Highlights assets with expired warranties
* Green background and a warning icon to draw attention to potential issues
