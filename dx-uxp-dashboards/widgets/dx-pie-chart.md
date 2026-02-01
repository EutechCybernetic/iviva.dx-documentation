# DX Pie Chart

### 1. Introduction

<figure><img src="../../.gitbook/assets/web and mobile (10).png" alt=""><figcaption></figcaption></figure>

The **DX Pie Chart** widget is designed to give users a clear and colorful breakdown of how data entries are distributed across different categories within a DX application. It is especially useful for visualizing proportional data, such as the number of issues by type, tasks by status, or requests by category.

***

### 2. What Does It Show?

The widget displays a pie chart where each slice represents a unique value from a selected field in the DX application. The size of each slice indicates the number of transactions associated with that value, helping users easily compare quantities at a glance.

***

### 3. Where Does the Data Come From?

This widget supports the following data sources:

* **ivivaDX** – Default internal source of DX application data.
* **API** – Pulls data from a configured external API.
* **iviva Service** – Uses a backend service to retrieve custom data.
* **Lucy** – Enables data to be retrieved from a low-code platform

> For this guide, we focus only on the **iviva DX** data source configuration, as others have been explained elsewhere.

***

### 4. Data Source Component Breakdown (ivivaDX Only)

<figure><img src="../../.gitbook/assets/1 - 2025-06-06T231903.705.png" alt=""><figcaption></figcaption></figure>

**Component 1: DX Application**\
Allows users to select the relevant DX application (e.g., Work Request) from which the pie chart will gather its data.

**Component 2: Base Field**\
Specifies which field’s values should be used to create the slices of the pie chart. For example, choosing "ProblemTitle" means each unique problem title becomes a slice.

**Component 3: Filter Query (IQL)**\
An optional filter where users can narrow down the dataset by entering specific conditions. This helps focus the chart on only relevant transactions.

***

### 5. General Details Component Breakdown

<figure><img src="../../.gitbook/assets/1 - 2025-06-06T231915.033.png" alt=""><figcaption></figcaption></figure>

**Component 1: Title**\
The name that appears at the top of the widget. It helps users identify what the pie chart represents (e.g., "Pie Chart Title").

**Component 2: Color Set**\
Determines the set of colors used for the pie slices. This improves clarity and visual distinction between segments.

***

### 6. Chart Details

<figure><img src="../../.gitbook/assets/1 - 2025-06-06T232255.937.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/1 - 2025-06-06T232439.102.png" alt=""><figcaption></figcaption></figure>

**Component 1: Enable Legend**\
Turns on or off the legend display. When enabled, it shows labels and color codes for each slice outside the chart.

**Component 2: Legend Position**\
Lets users choose where the legend should appear: Top, Bottom, Left, or Right of the chart.

**Component 3: Sort by Value**\
When enabled, the chart arranges slices from largest to smallest based on their count, making it easier to spot the most significant categories.

**Component 4: Outside Label Configuration**\
Controls labels that appear outside the pie slices:

* **Enable Label**: Activates outside labeling.
* **Label**: Defines the format (e.g., just name, value, or both).
* **Minimum Percentage to Show Label**: Hides labels for slices too small to display.
* **Thousands Separator**: Formats numbers with separators for better readability.
* **Enable Symbol**: Adds a symbol (e.g., "$") to values, either before or after the number if this is enabled.
  * **Symbol Label**: This is where you enter the actual symbol you want to display.
  * **Symbol Position**: Choose whether the symbol appears **before** or **after** the value.

**Component 5: Inside Label Configuration**\
Controls labels shown inside the slices. These settings mirror the outside label options and offer flexibility in how the data appears within the chart.

* **Enable Label**: Activates outside labeling.
* **Label**: Defines the format (e.g., just name, value, or both).
* **Minimum Percentage to Show Label**: Hides labels for slices too small to display.
* **Thousands Separator**: Formats numbers with separators for better readability.
* **Enable Symbol**: Adds a symbol (e.g., "$") to values, either before or after the number if this is enabled.
  * **Symbol Label**: This is where you enter the actual symbol you want to display.
  * **Symbol Position**: Choose whether the symbol appears **before** or **after** the value.

**Component 6: Enable Tooltip**\
Adds interactive tooltips on hover, showing the name and count of each slice.

**Component 7: Tooltip Display Options**

* **Thousands Separator**: Adds separators to values inside the tooltip.
* **Enable Symbol**: Allows a custom symbol (like "$") in the tooltip values if this is enabled.
  * **Symbol Label**: This is where you enter the actual symbol you want to display.
  * **Symbol Position**: Choose whether the symbol appears **before** or **after** the value.

***

### 7. Display Options

The pie chart includes several customizable display elements:

* **Legends**: Helps identify each slice.
* **Outside and Inside Labels**: Provide flexible, formatted text on or around slices.
* **Symbols and Prefixes/Suffixes**: Custom markers like currency symbols can be added to values.
* **Interactive Tooltip**: Displays real-time info when hovering over a slice.

***

### 8. Dashboard Visual Breakdown&#x20;

<figure><img src="../../.gitbook/assets/1 - 2025-06-06T232859.325.png" alt=""><figcaption></figcaption></figure>

The live widget on the dashboard visually presents data using a combination of labeled slices, interactive elements, and a legend. Here's how each part works:

**Component 1: Chart Title**\
Displays the title of the pie chart.\
This title can be customized based on the context or data being presented, as explained earlier.

**Component 2: Pie Chart Display**\
This is the central circular chart that shows each category as a colored slice. Each slice represents a unique value from the chosen field (e.g., problem types), and its size reflects the number of related transactions.

**Component 3: Slice Labels (Outside)**\
Some values appear **outside the chart**, like "Water leakage ($2)". These labels can include formatted numbers and optional symbols such as "$", and are configured under the **Outside Label Configuration** section.

**Component 4: Slice Labels (Inside)**\
Some values are shown directly **inside the slices** (e.g., "Frequent Circuit Breaker Trips (04)"). These are controlled via the **Inside Label Configuration**, and can include just names, just values, or both. Visibility is determined by the minimum percentage setting.

**Component 5: Legend Panel**\
Displayed on the **left side** of the chart, the legend lists each slice’s label with its corresponding color. This helps users quickly match what each slice represents without relying only on the chart.

**Component 6: Tooltip Popup**\
When hovering over a slice, a tooltip appears (e.g., "Thermostat Unresponsive: $1"). This tooltip gives a quick summary, and includes the value with formatting and symbol, as configured in the **Tooltip Settings**.
