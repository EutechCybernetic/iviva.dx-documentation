# DX Line Chart

#### 1. **Introduction**

<figure><img src="../../.gitbook/assets/web and mobile (3).png" alt=""><figcaption></figcaption></figure>

The **DX Line Chart** **widget** helps you visualise trends in your data across a selected category or over time. It displays connected points for each data group, making it ideal for spotting performance changes, usage patterns, or comparative trends across departments, users, or issues.

***

#### 2. **What Does It Show?**

This widget draws lines to represent how values change across a selected field. Each point along the line corresponds to a specific value of the chosen field, and multiple lines are displayed if data is grouped by another field (e.g., user or department). It’s perfect for showing comparisons like task trends by assignee or issue category over time.

***

#### 3. **Where Does the Data Come From?**

The widget supports the following data sources:

* **IvivaDX** – Default internal source of DX application data.
* **API** – Pulls data from a configured external API.
* **Iviva Service** – Uses a backend service to retrieve custom data.
* **Lucy** – Enables data to be retrieved from a low-code platform

> In this example, we focus on the **ivivaDX date source configuration**, which lets you select the application, base field, grouping field, and optional time range.
>
> For this guide, we focus only on the **Iviva DX** data source configuration, as others have been explained elsewhere.

***

#### 4. **Data Source Component Breakdown (IvivaDX only)**

<figure><img src="../../.gitbook/assets/1 - 2025-06-06T235153.939.png" alt=""><figcaption></figcaption></figure>

**Component 1: DX Application**\
Choose which IvivaDX application to use (e.g., _Work Request_). This determines which data records are available.

**Component 2: Filter Query (IQL)**\
Enter a filter condition to limit which records are used in the chart. This is optional but useful for narrowing the results.

**Component 3: Use a DateTime Field**\
Toggle this **ON** to group the data by a time-based field (e.g., Created Date). Turning it **OFF** allows grouping by other fields.

**Component 4: Base Field**\
Define the main X-axis grouping field.&#x20;

* If the DateTime toggle is ON, only time fields are available
* If OFF, you can choose from any suitable field like “Problem Title.”

**Component 5: Date Range**\
This appears only if the DateTime toggle is ON. Select a range like “Last 30 Days” or “This Week” to define which records appear in the chart.

**Component 6: Use Multiple Series**\
Enable this if you want to break down data into multiple series (e.g., by Assignee). Each series will be a separate line.

**Component 7: Series Field**\
Select which field to use for separating the series (e.g., Assignee or Department).

**Component 8: Series Options**\
Choose which values from the selected Series Field appear in the chart (e.g., Admin User, DihasL).

***

#### 5. **General Details Component Breakdown**

<figure><img src="../../.gitbook/assets/1 - 2025-06-06T235407.733.png" alt=""><figcaption></figcaption></figure>

**Component 1: Title**\
Enter a chart title to be displayed at the top of the widget. This helps users understand what the chart represents.

**Component 2: Color Set**\
Choose a color scheme for the chart lines. This is useful when displaying multiple series to distinguish them clearly.

***

#### 6. **Chart Details**



<figure><img src="../../.gitbook/assets/1 - 2025-06-07T002935.945.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/1 - 2025-06-07T003121.158.png" alt=""><figcaption></figcaption></figure>

**Component 1: X Axis Settings**

* **X Axis Position** – Choose top or bottom positioning.
* **Title** – Optional label displayed along the X-axis.
* **Label Rotation Value** – Rotate the labels for better visibility.
* **Label Interval Value** – Space out the labels.
* **Label Clip After Value** – Truncates long labels for a cleaner layout.

**Component 2: Y Axis Settings**

* **Y Axis Position** – Choose left or right positioning.
* **Title** – Optional label for the Y-axis.
* **Label Interval Value** – Controls spacing between numeric ticks.

**Component 3: Enable Legend**

* Toggles the legend panel on or off.
* **Legend Position** – Choose where the legend appears (Top, Bottom, Left, Right).

**Component 4: Chart Grid Settings**

* **Enable Grid X Axis** – Shows grid lines across vertical bars.
* **Enable Grid Y Axis** – Shows horizontal grid lines behind the bars.

**Component 5: Enable Tooltip**\
Displays a small popup with the exact values when hovering over a bar.

***

#### 7. **Display Options**

The **DX Line Chart widget** offers a dynamic and responsive charting interface. Based on the configuration, it may appear with the following display behaviors:

* **Single or Multiple Series:** The chart can display a single line for overall trends or multiple lines to compare groups (e.g., users or departments) side by side.
* **Time-based or Categorical View**: If a date field is selected, the X-axis shows intervals (e.g., days, weeks). If another field is used, the X-axis will show field values (e.g., issue types or locations).
* **Legends**: If enabled, the legend appears around the chart (top, bottom, left, or right), helping users identify groups by color.
* **Tooltip on Hover**: When enabled, hovering over the lines displays a tooltip with exact counts and category names.
* **Grid Lines**: Optionally show grid lines along the X and Y axes to improve readability.
* **Color Themes**: The color scheme used for bars is customizable in the widget's settings.

***

#### 8. **Dashboard Visual Breakdown**

<figure><img src="../../.gitbook/assets/1 - 2025-06-06T235933.014.png" alt=""><figcaption></figcaption></figure>

The **DX Line Chart** displays information in a clear and structured layout. Below is a component-wise explanation based on the example dashboard view:

* **Component 1: Title**\
  The chart title appears at the top of the widget (e.g., "LINE CHART TITLE"). This title is customizable from the configuration.
* **Component 2: Colored Lines (Data Series)**\
  Each colored line represents a selected group or series (e.g., "Admin User", "DihasL"). The color theme used is defined in the configuration.
* **Component 3: X-Axis (Base Field Values)**\
  The horizontal axis shows categories or time intervals based on the selected base field. In the example, it displays issue types such as “Water leak” and “Office Lights Flickering”.
* **Component 4: Y-Axis (Values)**\
  The vertical axis displays numerical values that correspond to each field on the X-axis.
* **Component 5: Legend**\
  The legend appears on the left and maps each series to its line color, helping users understand which group each line represents.
* **Component 6: Data Points and Lines**\
  Each point marks a specific value in the dataset, and the lines connect these points to illustrate the trend across the selected categories.
* **Component 7: Tooltip on Hover**\
  When you hover over a line, a tooltip appears showing the exact count at that point.\
  This provides quick, detailed insights without needing to refer to the legend.
