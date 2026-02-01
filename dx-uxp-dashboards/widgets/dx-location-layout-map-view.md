# DX Location Layout Map View

#### **1. Introduction**

<figure><img src="../../.gitbook/assets/web and mobile4 (2).png" alt=""><figcaption></figcaption></figure>

**The DX Location Layout Map widget visually represents the physical layout of any defined area in your DX environment—like a site, building, floor, or office.** It helps users get a sense of how a location is organised by displaying its layout on an interactive map. This is especially useful in complex environments like campuses, industrial sites, or large facilities where visual context is important for better navigation, operations, planning, or wayfinding.

***

#### **2. What Does It Show?**

The **DX Location Layout Map** widget displays the selected **layout map** of a location, such as a building or facility area. Depending on the chosen layout category, it can show layouts like floor plans, zone maps. Users can choose to show either location-based layouts (_e.g., for buildings like “mda” or “building 1”_) or asset-based layouts.

For example, imagine a parent location called **mda** has a sub-location called **mda.building1**. In the DX Map View, clicking the pin for **mda** opens a popup with basic information. Clicking the link in that popup takes the user to the location portal, where this widget appears and shows the layout for **mda**.

***

#### **3. Where Does the Data Come From?**

{% hint style="info" %}
The **DX Location Layout Map** widget does not need users to set up any external data sources like **iviva.DX, APIs, iviva Service,** or **Lucy.** All the layout data is internally pulled automatically from the selected **layout category** linked to the chosen location or asset. The system handles this automatically in the background once a layout category is selected.
{% endhint %}

***

#### **4. Data Source Component Breakdown**

{% hint style="info" %}
&#x20;The **DX Location Layout Map** widget does **not** use any separate data source configuration panels. That means there is no need to set up iviva.DX, API, iviva Service, or Lucy connectors.
{% endhint %}

***

#### **5. General Details Component Breakdown**

<figure><img src="../../.gitbook/assets/1 - 2025-06-10T132132.485.png" alt=""><figcaption></figcaption></figure>

In the configuration panel, users can customise the widget using the following options:

*   **Component 1: Dashboard Type**

    A dropdown where users choose whether the widget shows layouts for a **Location** or **Asset**

    * Selecting **Location** shows the layout of locations.
    * Selecting **Asset** shows where assets are placed within the layout.
* **Component 2: Layout Category**\
  A required selector that lets users pick from available layout categories (e.g., Portal) already set up in the system.
* **Component 3: Enable Red Pin**\
  A checkbox that, when ticked, shows a red pin on the layout to mark the exact spot of the selected location or asset.
* **Component 4: Overwrite Title**\
  This checkbox lets users replace the default widget title. When enabled, a text box appears below where users can enter a custom title.
* **Component 5: Custom Title Text Box**\
  Only visible when Overwrite Title is enabled. Users can type a custom title here, which will appear in the widget header instead of the system-generated one.

***

#### **6. Display Options**

The display options are handled automatically based on the selected **dashboard type** and **layout category**. Visual changes include:

* Displaying either a location or asset layout, depending on the user's selection
* Showing a red pin to highlight the active location or asset
* Displaying a custom widget title, if one is set

These configurations allow users to personalise how the layout map appears, making it easier to interpret based on their roles and needs.

***

#### **7. Dashboard Visual Breakdown**

<figure><img src="../../.gitbook/assets/1 - 2025-06-10T132633.514.png" alt=""><figcaption></figcaption></figure>

**Component 1: Widget Title**\
Displays the title of the widget, which can either be the system default or a custom name set by the user during configuration

**Component 2: View Selector (Map View / Overview)**\
Lets users switch between two display modes:

* **Map View** shows the actual layout or floor plan visually
* **Overview** provides textual or summarised details about the location layout.

**Component 3: Zoom Controls**\
Plus (+) and minus (−) buttons allow users to zoom in or out for a closer or wider view of the layout.

**Component 4: Layout Display Area**\
The main display area where the selected layout is shown. It shows zones, rooms, or other defined sections based on the selected layout.

**Component 5: Red/Blue Pin Indicator**\
A red or blue pin appears (depending on configuration) to mark the exact location or asset on the map, helping users quickly spot the point of interest.
