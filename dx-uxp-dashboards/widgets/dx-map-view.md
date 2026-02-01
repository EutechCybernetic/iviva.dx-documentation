# DX Map View

#### 1. Introduction

<figure><img src="../../.gitbook/assets/web and mobile (7).png" alt=""><figcaption></figcaption></figure>

The **DX Map View** widget displays an **interactive map** centered on a specific geographic location. It allows users to visualise areas on the map by specifying coordinates, zoom levels, and an optional custom tile map URL. \
This widget is ideal for dashboards that require a **geographic context** or **location-based insight**.

***

#### 2. What Does It Show?

The widget displays a map centered on a configured location, showing surrounding geographic details according to the selected **zoom level**. Users can interact with the map using built-in **zoom controls** to explore the area in more detail.

***

#### 3. Where Does the Data Come From?

{% hint style="info" %}
No data source needs to be configured for this widget. Instead, users set up a visual map view by entering location coordinates and visual preferences manually.
{% endhint %}

***

#### 4. Data Source Component Breakdown

{% hint style="info" %}
**Not applicable** – this widget does not require a data source connection.
{% endhint %}

***

#### 5. General Details Component Breakdown

<figure><img src="../../.gitbook/assets/1 - 2025-06-07T094458.501.png" alt=""><figcaption></figcaption></figure>

**Component 1: Title**\
This is the label that appears at the top of the widget on the dashboard. It helps identify what the map is showing (e.g., “Africa”).

**Component 2: Leaflet Map URL**\
This is the source URL used to render the map tiles. The default option provided uses OpenStreetMap. Advanced users may change this if they prefer an alternative map tile service.

**Component 3: Map Center Position - Latitude**\
Specifies the **latitude** (north-south position) where you want the map to be centered. Valid values range from -90 to +90.

**Component 4: Map Center Position -Longitude**\
Specifies the **longitude** (east-west position) where you want the map to be centered. Valid values range from -180 to +180.

**Component 5: Map Zoom Size**\
Controls how zoomed in the map should appear by default. A lower value (e.g., 1–3) shows a broader view, while higher values zoom into specific locations.

***

#### 6. Display Options

* **Map View**: \
  The map is **interactive** and scrollable. Users can zoom in and out using the **plus** (+) and **minus** (−) buttons on the map.
* **Customizable Zoom and Center**: \
  The map display adjusts dynamically based on the entered **latitude**, **longitude**, and **zoom level**.
* **Optional Tile Source**: \
  Users may provide their own tile map URL if they wish to use a custom map styling.

***

#### 7. Dashboard Visual Breakdown

<figure><img src="../../.gitbook/assets/1 - 2025-06-07T094756.653.png" alt=""><figcaption></figcaption></figure>

**Component 1: Title**\
Appears above the map. In this example, it is labeled as “AFRICA”, representing the view shown.

**Component 2: Zoom Controls**\
Located on the top-left corner of the map, these **plus** (+) and **minus** (−) buttons allow users to zoom in and out as needed.

**Component 3: Map Display**\
This section displays the interactive map view. It centers based on the specified **latitude** and **longitude**. In the current example, the map is centered on the African continent with standard OpenStreetMap tiles.
