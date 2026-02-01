# Location Dashboard

<figure><img src="../.gitbook/assets/web and mobile (1) (4) (1).png" alt=""><figcaption></figcaption></figure>

The **Location Dashboard** provides an in-depth view of a **specific facility** selected from the Portfolio Dashboard. While the Portfolio Dashboard offers a high-level, multi-facility overview, the Location Dashboard zooms in on a **single site**, displaying its individual performance, associated locations, and relevant operational insights.

This dashboard enables users to monitor localized activity, view contextual layouts or photos of the facility, and manage location-specific requests and assets.

***

### 🗺️ What Does It Show?

* &#x20;**Location Layout Map:** Visually represents the selected facility. Depending on the configuration, this may appear as:
  * A layout (such as a floor plan or image), or
  * A geographic pin indicating the facility's position on the map.
* **Real-time Summary**: Displays:
  * Number of child locations (e.g., internal offices or subdivisions)
  * Total, common, and commercial area metrics
* **Key Workload Indicators**:
  * Number of Work Requests
  * Corrective Work Orders
  * Active Service Orders

If the facility contains child locations, they may also appear on the map. Selecting a child location navigates users to its corresponding **Location Dashboard**.

***

### 🔁 How It Connects to Portfolio Dashboard

From the **Portfolio Dashboard**, selecting a facility marker redirects the user to the **Location Dashboard**, providing focused insight into the selected site.

While it uses the same widget types for a consistent user experience, the content is tailored for the specific facility and may reflect different configurations such as:

* Layout image vs. geographical map
* Different child location structure
* Site-specific assets or application links

***

### 🧩 Key Components

#### 🗺️ Location Layout Map

Displays the selected facility's layout or map-based view. This component is configurable and can represent either:

* An internal layout (e.g., site photo or schematic), or
* The facility’s location on a geographic map\
  Child locations—if configured—appear as markers on the map and can be clicked to open their individual **Location Dashboards**.

#### 📊 Facility Statistics

* **Child Locations**: Displayed in the sidebar and also shown on the map (if applicable)
* **Area Metrics**: Includes Total, Common, and Commercial areas (measured in m²)
* **Workload Indicators**: Tile widgets display real-time counts of key operational metrics

#### 📁 Sidebar with Toggle

Similar to the **Portfolio Dashboard**, the sidebar includes a toggle that lets users switch views:

* **Child Locations View**: Displays immediate sub-locations within the current facility
* **Applications/Assets View**: Switches to show UXP application links or pinned asset sets related to this facility

***

### 📱 Responsive Design

The dashboard works consistently across both **web** and **mobile** platforms:

* The layout/map scales appropriately to fit the screen size.
* The sidebar and summary widgets remain scrollable and fully accessible.
* Navigation between dashboards, whether from parent to child or back to the Portfolio Dashboard is seamless.

***

### 🧰 Powered by UXP Widgets

The **Location Dashboard** leverages reusable, no-code widgets for fast configuration and deployment:

* **DX Location Layout Map**
* **DX Portfolio Sidebar**
* **DX Tile Cards**

Its architecture ensures consistency across all facilities, while still allowing for location-specific customization.
