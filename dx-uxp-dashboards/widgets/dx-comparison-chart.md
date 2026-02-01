# DX Comparison Chart

#### 1. Introduction

<figure><img src="../../.gitbook/assets/web and mobile (13).png" alt=""><figcaption></figcaption></figure>

The **DX SLA Comparison Chart** widget offers a clear, visual way to compare the proportion of transactions that met or missed their Service Level Agreements (SLAs) over a chosen period. This helps teams track performance and identify patterns that may affect timely response or resolution of work.

***

#### 2. What Does It Show?

This widget displays:

* Two circular gauges that show the percentage of transactions completed _within SLA_ (in green) and _outside SLA_ (in red) for both **Respond** and **Resolve** stages.
* A line chart beneath the gauges, which tracks how many transitions were completed _in_ and _out_ of SLA over time.
* The time scale can be switched between **Year**, **Month**, **Week**, or **Day** for a detailed or summarized view.
* A filter icon opens a popup that lets users narrow down the chart to show only certain **transaction priorities**.

***

#### 3. Where Does the Data Come From?

This widget supports data from:

* **ivivaDX** – Default internal source of DX application data.
* **API** – Pulls data from a configured external API.
* **iviva Service** – Uses a backend service to retrieve custom data.
* **Lucy** – Enables data to be retrieved from a low-code platform

> For this guide, we focus only on the **iviva DX** data source configuration, as others have been explained elsewhere.

***

#### 4. Data Source Component Breakdown (ivivaDX only)

<figure><img src="../../.gitbook/assets/1 - 2025-06-09T023932.809.png" alt=""><figcaption></figcaption></figure>

**Component 1: DX Application**

* Lets users select the specific DX application (e.g., Work Request) from which SLA data should be pulled.

**Component 2: Filter Query (IQL)**

* Optional field where users can enter specific filter conditions to refine which transactions are considered in the chart.

***

#### 5. General Details Component Breakdown

<figure><img src="../../.gitbook/assets/1 - 2025-06-09T024054.784.png" alt=""><figcaption></figcaption></figure>

**Component 1: Title**

* Sets the title of the widget as shown on the dashboard (e.g., "SLA In and Out").

**Component 2: X Axis Label Interval**

* Optional setting to control how frequently labels appear on the time axis of the line chart. This helps manage label clutter when viewing dense datasets.

***

#### 6. Display Options

* Users can switch between **Year**, **Month**, **Week**, or **Day** view to control the time resolution.
* The filter icon at the top right corner opens a panel where users can apply filters such as **transaction priority**.
* Color coding:
  * Green line and progress: In SLA
  * Red line and progress: Out SLA

***

#### 7. Dashboard Visual Breakdown

<figure><img src="../../.gitbook/assets/1 - 2025-06-09T024307.975.png" alt=""><figcaption></figcaption></figure>

The dashboard view includes:

**Component 1: Widget Title and Time Range Selection**

* The title **"SLA IN AND OUT"** appears at the top.
* Right below the title, there are time range buttons: **YEAR**, **MONTH**, **WEEK**, and **DAY**.
* These let you choose the time scale for the data displayed in the chart below.

**Component 2: Filter Icon**

* Located at the top-right corner of the widget.
* Clicking it opens a popup where users can filter the results shown in the chart based on **transaction priority**, allowing for more focused insights.

**Component 3: SLA Percentage Gauges**

* Two circular gauges labeled **Respond** and **Resolve**.
* These show the percentage of transitions that were completed within SLA for each stage.
* For example, Respond shows **56%**, meaning 56% of respond transitions happened within the SLA target time.

**Component 4: Line Chart**

* A line chart displays how many transitions were completed _In SLA_ (green line) and _Out SLA_ (red line) across different months.
* The vertical axis shows the number of transitions (transition count), while the horizontal axis lists the months of the year.
* Each point in the graph shows how SLA performance varied over time, helping users quickly identify spikes or drops in performance.

**Component 5: SLA Type Labels in the Graph Legend**

* At the bottom of the chart, the legend explains the two color-coded lines:
  * **Green** for _In SLA_
  * **Red** for _Out SLA_



This visualisation helps teams monitor SLA performance trends and prioritize improvements accordingly.
