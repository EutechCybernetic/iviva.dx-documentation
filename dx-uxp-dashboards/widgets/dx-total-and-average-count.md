# DX Total & Average Count

### 1. Introduction

<figure><img src="../../.gitbook/assets/web and mobile5 (1).png" alt=""><figcaption></figcaption></figure>

The **DX Total & Average Count** widget summarises numeric data by displaying the **total** and **average** values from a number field you choose. It is great for highlighting key figures—like total requests, average costs, or performance indicators—from any DX application you choose.

***

### 2. What Does It Show?

The DX Total & Average Count widget shows two key values:

* **Total**: the sum of all values from the selected number field
* **Average**: the average across all matching records

These metrics are shown in a clean and bold format, so it is easy for users to spot cumulative and mean values at a glance. You can customise the titles, colours, and visibility of each metric.

***

### 3. Where Does the Data Come From?

This widget supports four data sources:

* **iviva.DX** – the default internal source for DX application data
* **API** – pulls data from a configured external API
* **iviva Service** – uses a backend service to fetch custom data
* **Lucy** – enables data to be retrieved from a low-code platform

> In this guide, we are covering how to set up the **iviva.DX** data source only.

***

### 4. Data Source Component Breakdown (iviva.DX only)

<figure><img src="../../.gitbook/assets/1 - 2025-06-09T014021.801.png" alt=""><figcaption></figcaption></figure>

The iviva.DX data source setup includes the following components:

**Component 1: DX Application**\
Choose the DX application where the number field will be retrieved _(e.g., Work Request_).

**Component 2: Base Field**\
Select the specific number field within the chosen application to calculate the total and average values (_e.g., Number)_.

**Component 3: Filter Query (IQL)**\
An optional field that lets you set conditions to narrow down the data used in calculations. For example, you might filter to include only "Open" records if needed.

***

### 5. General Details Component Breakdown

<figure><img src="../../.gitbook/assets/1 - 2025-06-09T014312.324.png" alt=""><figcaption></figcaption></figure>

These components let you customise how the total and average values appear:

**Component 1: Title**\
Sets the main title at the top of the widget (_e.g., Number Field)_

**Component 2: Enable Total**\
Select the **Enable Total** checkbox to show the total value. If selected, it appears with its own title

**Component 3: Total Title**\
Custom label for the total (_e.g., Total)_

**Component 4: Enable Average**\
Select the **Enable Average** checkbox to show the average value. You can choose to show only total, only the average, or both

**Component 5: Average Title**\
Custom label for the average (_e.g., Average_)

**Component 6: Background Colour**\
Choose a background colour for the widget

**Component 7: Sub Title Colour**\
Sets the colour for subtitles like 'TOTAL' and 'AVERAGE'

**Component 8: Text Colour**\
Controls the colour of the main numeric values (_e.g., '25' or '2.50%'_)

***

### 6. Display Options

The widget has a compact but informative layout. You can:

* Choose to show the **Total**, **Average**, or both
* Set **custom titles** for each metric
* Customise **background, subtitle, and text colours**
* Apply **filters** to control which data gets included in the calculation

***

### 7. Dashboard Visual Breakdown

<figure><img src="../../.gitbook/assets/1 - 2025-06-09T014501.788.png" alt=""><figcaption></figcaption></figure>

Here is how each part of the widget appears when appears on the dashboard:

**Component 1: Widget Title**\
"NUMBER FIELD" appears at the top, based on the configured title

**Component 2: Total Value Section**\
Shows the label "TOTAL" followed by the computed total (e.g., 25), styled and aligned for clarity

**Component 3: Average Value Section**\
Appears at the bottom right with the configured label "AVERAGE" and its values (e.g., 2.50%), either as a percentage or a numeric value

The layout is optimised for quick scanning and easy visibility on dashboards, especially when placed alongside other number-based widgets.
