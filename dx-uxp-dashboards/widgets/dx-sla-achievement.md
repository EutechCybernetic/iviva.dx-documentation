# DX SLA Achievement

### 1. Introduction

<figure><img src="../../.gitbook/assets/web and mobile6.png" alt=""><figcaption></figcaption></figure>

The **DX SLA Achievement** widget is designed to help teams monitor their service level performance by visualising how effectively they are meeting response and resolution times. This widget offers a quick and clear breakdown of whether actions were completed **early**, **on time**, or **overdue**, allowing users to track service quality and adherence to commitments.

***

### 2. What Does It Show?

This widget displays a **horizontal bar chart** showing the percentage of requests that were handled in three time categories:

* **Early**: Completed before the SLA deadline
* **On Time**: Completed exactly within the SLA timeframe
* **Overdue**: Completed after the SLA deadline

The chart is divided into two rows:

* **Respond** SLA achievement
* **Resolve** SLA achievement

Each row is colour-coded (green for Early, yellow for On Time, red for Overdue) and labeled with percentage values for easy interpretation.

***

### 3. Where Does the Data Come From?

The widget supports the following data sources:

* **iviva.DX** – Default internal source of DX application data
* **API** – Pulls data from a configured external API
* **Iviva Service** – Uses a backend service to retrieve custom data
* **Lucy** – Enables data retrieval from a low-code platform

> For this guide, we focus only on the i**viva.DX** data source configuration, as the others have been covered elsewhere.

The actual SLA status values are derived from the selected application's SLA-related metrics.

***

### 4. Data Source Component Breakdown (iviva.DX only)

<figure><img src="../../.gitbook/assets/1 - 2025-06-09T021849.635.png" alt=""><figcaption></figcaption></figure>

This section outlines the fields visible when selecting iviva.DX as the data source:

**Component 1: DX Application**\
Select the relevant DX application (e.g., _Work Request_) whose SLA data should be used in the widget. This application must have SLA tracking enabled for meaningful results.

***

### 5. General Details Component Breakdown

<figure><img src="../../.gitbook/assets/1 - 2025-06-09T021944.864.png" alt=""><figcaption></figcaption></figure>

This section configures the title shown in the widget display.

**Component 1: Title**\
Sets the title of the widget (e.g., _SLA Achievement_). This title appears at the top of the chart to help users identify the context of the SLA breakdown.

***

### 6. Display Options

The widget offers the following visual and functional features:

* **SLA Type Segmentation**: Separates results into 'Respond' and 'Resolve' phases
* **Colour Coding**: Uses intuitive colours to differentiate SLA statuses:
  * Green: Early
  * Yellow: On Time
  * Red: Overdue
* **Percentage Labels**: Displays exact percentage values on each chart segment
* **Compact Layout**: Designed for easy embedding in dashboards without clutter

There are no additional configurable display options in the settings panel—visuals are generated automatically from the data.

***

### 7. Dashboard Visual Breakdown

<figure><img src="../../.gitbook/assets/1 - 2025-06-09T022119.451.png" alt=""><figcaption></figcaption></figure>

Here is how the widget appears when live on the dashboard.

**Component 1: Widget Title – “SLA ACHIEVEMENT”**\
Displayed at the top of the widget, as configured in the General Details

**Component 2: Horizontal SLA Bars**

* Each row represents a phase: “Respond” and “Resolve.”
* Each row is segmented by SLA outcome:
  * Green bar for Early (e.g., “36.36%”)
  * Yellow bar for On Time (e.g., “9.09%”)
  * Red bar for Overdue (e.g., “54.55%”)

**Component 3: Legend Panel**\
Shown at the bottom of the chart, this panel explains the meaning of each colour-coded segment:

* 🟩 Early
* 🟨 On Time
* 🟥 Overdue

This visual guide ensures quick understanding of SLA performance across key service stages.
