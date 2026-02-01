# DX Bar Chart

**1. Introduction**

<figure><img src="../../.gitbook/assets/web and mobile (1) (2) (1).png" alt=""><figcaption></figcaption></figure>

The **DX Bar Chart** widget is a visual analytics tool that displays categorized transaction data from a DX application in a clear bar chart format. It is designed to help users compare values, identify trends, and make sense of grouped data across different time frames or attributes. Whether analysing task completion by assignee or comparing equipment fault types, this widget turns numbers into meaningful visuals.

The widget is supported across both web and mobile dashboards, offering a consistent and responsive user experience.

***

**2. What Does It Show?**

When added to a dashboard, the **DX Bar Chart** widget displays a vertical or horizontal bar chart representing grouped transaction data.

Each bar corresponds to a specific category or field value (such as assignees or issue types), and the height of the bar reflects the number of matching records. When grouping is enabled, each category is further split by group values (e.g., multiple users or statuses) and shown in color-coded segments.

Hovering over any bar reveals a tooltip showing the count for each group in that category. Legends are displayed alongside the chart to identify what each color represents.

***

**3. Where Does the Data Come From?**

The DX Bar Chart widget supports multiple data sources:

* **ivivaDX** – Default internal source of DX application data.
* **API** – Pulls data from a configured external API.
* **iviva Service** – Uses a backend service to retrieve custom data.
* **Lucy** – Enables data to be retrieved from a low-code platform

> In this example, we focus on the **ivivaDX** source configuration, which lets you select the application, base field, grouping field, and optional time range.
>
> For this guide, we focus only on the **iviva DX** data source configuration, as others have been explained elsewhere.

***

**4. Data Source Component Breakdown (ivivaDX Only)**

<figure><img src="../../.gitbook/assets/1 - 2025-06-06T220113.375.png" alt=""><figcaption></figcaption></figure>

**Component 1: DX Application**\
Select the application from which transaction data should be pulled (e.g., "Work Request").

**Component 2: Filter Query (IQL)**\
Allows entry of advanced conditions to filter records based on business rules.

**Component 3: Use a DateTime Field Toggle**\
This switch lets you decide whether to group the chart data by time.

* When **enabled**, the chart groups transactions based on a date-related field (like `TargetStartDate`). This is useful for showing trends across a time range such as “Current Week” or “Last 30 Days.”
* When **disabled**, you can select any other type of field—such as “Problem Title” or “Department”—to group the data instead.

**Component 4: Base Field**\
This is the main field used for grouping transactions along the X-axis.

* If **Use a DateTime Field** is turned **on**, only date or time fields can be selected here.
* If it's **off**, this dropdown will show all other available fields, allowing flexible categorization based on your needs.

**Component 5: Date Range**\
When using a DateTime field, this option appears to let you define the time period for the chart (e.g., “Today,” “This Month,” “Last 30 Days”). It controls which transactions are included based on the selected date field.

**Component 6: Use Grouping Field Checkbox**\
Enables grouping (e.g., by user, status, department) within each X-axis category.

**Component 7: Grouping Field**\
Select the field to group by (e.g., "Assignee").

**Component 8: Grouping Options**\
Select which values of the grouping field to include in the chart (e.g., "Admin User", "DihasL").

***

**5. General Details Component Breakdown**

<figure><img src="../../.gitbook/assets/1 - 2025-06-06T220308.981.png" alt=""><figcaption></figcaption></figure>

**Component 1: Title**\
A customisable title for the widget, shown above the chart.

**Component 2: Color Set**\
Choose the color theme to be used for chart bars and group legends. Each grouping option will be shown in a different color.

***

**6. Chart Details**

<figure><img src="../../.gitbook/assets/1 - 2025-06-06T220539.788.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/1 - 2025-06-06T220907.004.png" alt=""><figcaption></figcaption></figure>

**Component 1: Group Mode**\
Controls how groups are visually arranged:

* Grouped – Separate bars for each group per category.
* Stacked – Groups stacked within a single bar.

**Component 2: X Axis Settings**

* **X Axis Position** – Choose top or bottom positioning.
* **Title** – Optional label displayed along the X-axis.
* **Label Rotation Value** – Rotate the labels for better visibility.
* **Label Interval Value** – Space out the labels.
* **Label Clip After Value** – Truncates long labels for a cleaner layout.

**Component 3: Y Axis Settings**

* **Y Axis Position** – Choose left or right positioning.
* **Title** – Optional label for the Y-axis.
* **Label Interval Value** – Controls spacing between numeric ticks.

**Component 4: Enable Legend**

* Toggles the legend panel on or off.
* **Legend Position** – Choose where the legend appears (Top, Bottom, Left, Right).

**Component 5: Chart Grid Settings**

* **Enable Grid X Axis** – Shows grid lines across vertical bars.
* **Enable Grid Y Axis** – Shows horizontal grid lines behind the bars.

**Component 6: Enable Tooltip**\
Displays a small popup with the exact values when hovering over a bar.

***

#### &#x37;**. Display Options**

The **DX Bar Chart** widget offers a dynamic and responsive charting interface. Based on the configuration, it may appear with the following display behaviors:

* **Grouped or Stacked View**: The chart can visually group or stack bars based on the configured mode (e.g., per user, per department, etc.).
* **Time-based or Categorical View**: If a date field is selected, the X-axis shows intervals (e.g., days, weeks). If another field is used, the X-axis will show field values (e.g., issue types or locations).
* **Legends**: If enabled, the legend appears around the chart (top, bottom, left, or right), helping users identify groups by color.
* **Tooltip on Hover**: When enabled, hovering over bars displays a tooltip with exact counts and category names.
* **Grid Lines**: Optionally show grid lines along the X and Y axes to improve readability.
* **Color Themes**: The color scheme used for bars is customisable in the widget's settings.

***

**8. Dashboard Visual Breakdown**

<figure><img src="../../.gitbook/assets/1 - 2025-06-06T221648.104.png" alt=""><figcaption></figcaption></figure>

**Component 1: Chart Title**\
Displays the title of the bar chart.\
This title can be customised based on the context or data being presented, as explained earlier.

**Component 2: Left-Hand Legend Panel**\
Displays color-coded labels to identify which bar segment belongs to which grouping option (e.g., user, department).\
This helps users understand how the chart is categorised.

**Component 3: The Bar Chart**\
Visually represents data as vertical bars.\
Each bar corresponds to a specific category and shows the count of transactions within that category.

**Component 4: Color-Coded Groupings**\
When grouping is enabled, each colored segment within a bar represents a different grouping value (e.g., different users or departments).\
This adds an extra layer of insight to the chart.

**Component 5: Tooltip on Hover**\
When you hover over a bar or segment, a tooltip appears showing the exact count for each group.\
This provides quick, detailed insights without needing to refer to the legend.
