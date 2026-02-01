# DX Transaction Info

#### 1. Introduction

<figure><img src="../../.gitbook/assets/web and mobile (15).png" alt=""><figcaption></figcaption></figure>

The **DX Transaction Info** widget gives you a quick snapshot of the latest transaction from a selected DX application. It is ideal for highlighting key information—such as issue title, status, or identifier—in a visual card format right on your dashboard. You can also display information about a specific transaction by passing the ID in the page URL as a query string (e.g., `?transactionId=WR20250608060`) and using a matching filter condition like `Id=#{transactionId}`.

***

#### 2. What Does It Show?

The DX Transaction Info widget displays a card with selected data fields from the latest transaction in a DX application. You can customise the displayed title, description, icons, chip labels, and background colour to suit your needs. The widget is great for spotlighting important updates like _Last Created Request, Latest Fault Ticket, or Recent Submission._

***

#### 3. Where Does the Data Come From?

The **DX Transaction Info** widget supports the i**viva.DX** data source only.\
It pulls data from a chosen DX app and lets you apply an optional query filter (IQL) to narrow down which transaction gets shown.

To target a specific transaction dynamically, you can add a filter like `Id=#{transactionId}` and pass the `transactionId` via the page URL.

***

#### 4. Data Source Component Breakdown

<figure><img src="../../.gitbook/assets/1 - 2025-06-11T094133.723.png" alt=""><figcaption></figcaption></figure>

**Component 1: DX Application**\
Choose the DX application you want the widget to pull data from (e.g., Work Request). This step is required.

**Component 2: Filter Query (IQL)**\
The Filter Query (IQL) is an optional filter used to refine the dataset. You can use this to pull in a specific transaction by applying a filter like `Id=#{transactionId}` and passing the `transactionId`  in the page URL.

***

#### 5. General Details Component Breakdown

<figure><img src="../../.gitbook/assets/1 - 2025-06-11T094317.651.png" alt=""><figcaption></figcaption></figure>

**Component 1: Enable Icon**\
Turns on the icon display for the transaction card

**Component 2: Icon Type Config**\
Set up one or more icons to show in the DX Transaction Info widget. Make sure at least one is marked as default.

**Component 3: Enable Headers**\
Shows the text headers on the transaction card—a main title and an optional description (sub-title) taken from the transaction data.

**Component 4: Main Title**\
This is the main info that stands out on the card, like an ID, reference number, or title.\
Click the pencil icon next to the field to open the Edit Field popup (see Component 5) and choose what to display.

**Component 5: Edit Field (Opens via Pencil Icon)**\
This popup appears when you edit fields like Main Title or Description. You can:

* **Rename the field title** (just for display)
* **Select the actual field** from the dataset you want to show
* **Choose the display type**—like single-line text or another format

This configuration controls how the field looks on the widget.

**Component 6: Description**\
Adds a secondary field below the main title—great for adding extra context to the transaction (e.g., problem summary).\
Uses the same Edit Field popup as the Main Title.

**Component 7: Enable Priority Chip**\
Displays a chip in the top-right corner of the card to show the transaction's priority (e.g., Low, Medium, High)

**Component 8: Background Colour**\
Lets you choose a fixed background colour for the transaction card. If you do not set one, it will use the priority colour—if the app has a priority field. This helps the widget stand out visually on the dashboard.

**Component 9: Enable Perform Transition**\
Adds a stage action button (_e.g., New, In Progress_) on the card. If turned on, users can click this button to perform a transition for the transaction right from the widget.

***

#### 6. Display Options

The DX Transaction Info widget is highly visual and easy to customise. You can style the card with features like:

* **Icons**: Add context or category indicators
* **Main Title & Description**: Pick meaningful fields to give clear summary
* **Priority Chip**: Shows how important the transaction is (e.g., Low, Medium, High)
* **Transitions**: Let users perform status transitions with a button
* **Colour Customisation**: Set the background to match your branding or urgency level

***

#### 7. Dashboard Visual Breakdown

<figure><img src="../../.gitbook/assets/1 - 2025-06-11T095316.494.png" alt=""><figcaption></figcaption></figure>

**Component 1: Main Title**\
Displayed in bold. In this example, `WR20250608040` is the request ID.

**Component 2: Description**\
Appears below the title—for example, '_Frequent Circuit Breaker Trips_' is shown here.

**Component 3: Priority Chip**\
Shows up in the top-right corner—like '_Low_' in this example

**Component 4: Icon**\
Appears on the left side of the card (_e.g., a document icon)_

**Component 5: Stage/Transition Button**\
Appears in the bottom-right corner—like “New” in this example—to show the current stage of the transaction. If transitions are enabled, this label can be clicked.

***
