# DX Related Assets

### 1. Introduction

<figure><img src="../../.gitbook/assets/web and mobile (11).png" alt=""><figcaption></figcaption></figure>

The **DX Related Assets** widget displays a list of assets that are linked to the current context—such as a selected location, asset, or record. It helps users quickly identify and access relevant equipment or resources that are part of or associated with the main item being viewed.

***

### 2. What Does It Show?

This widget shows a vertical list of related assets, each represented with a label, icon, and short description. Each item in the list includes:

* A **circular icon** with initials or identifiers
* The **asset name** (e.g., _Generator 01, Elevator B_)
* A **source label** (e.g., _mda_) that indicates where the asset belongs or originates
* A **pin icon** that lets users mark important assets, keeping them visible across the dashboard—such as the links section in the portfolio sidebar widget

***

### 3. Where Does the Data Come From?

{% hint style="info" %}
No data source needs to be configured for this widget.
{% endhint %}

***

### 4. Data Source Component Breakdown (iviva.DX only)

{% hint style="info" %}
There is **no configurable data source panel** for the iviva.DX option in this widget. When iviva.DX is selected, the widget automatically pulls related assets based on the current context. No additional setup is required from the user.
{% endhint %}

***

### 5. General Details Component Breakdown

This widget **does not contain a General Details configuration section**. It inherits the context and appearance directly from system defaults and the connected data source.

***

### 6. Display Options

The DX Related Assets widget features a simple, clean layout with the following display elements:

* **Asset Icons**: Coloured circles containing the initials of each asset for easy visual scanning
* **Pinned Assets**: Users can click the pin icon to keep certain assets readily accessible. Pinned items may appear in other parts of the system or remain highlighted.
* **Auto-update**: The list refreshes automatically based on the active context or user interactions within the dashboard.

***

### 7. Dashboard Visual Breakdown

<figure><img src="../../.gitbook/assets/1 - 2025-06-09T004804.933.png" alt=""><figcaption></figcaption></figure>

Below is an explanation of each visual element shown in the widget dashboard view:

**Component 1: Widget Title – “RELATED ASSETS”**\
Appears at the top of the widget and clearly identifies the purpose of the list

**Component 2: Asset Icon**\
A circular coloured icon with initials (e.g., _“GO” for Generator 01_) helps users quickly recognise the asset

**Component 3: Asset Name**\
Displays the name of each asset (e.g., _Printer, Elevator B_) in bold text for clarity

**Component 4: Source Label (e.g., “mda”)**\
Shown below the asset name, this label indicates the source or location group the asset belongs to

**Component 5: Pin Icon**\
A grey or filled pin icon on the right side allows users to pin or unpin the asset. Pinned assets may be grouped or highlighted elsewhere on the dashboard—such as in the links section in the Portfolio Sidebar widget.
