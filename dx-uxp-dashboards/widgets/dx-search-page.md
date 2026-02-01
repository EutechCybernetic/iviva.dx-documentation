# DX Search Page

#### 1. Introduction

<figure><img src="../../.gitbook/assets/web and mobile8.png" alt=""><figcaption></figcaption></figure>

The **DX Search Page** widget lets you browse and filter transactions from a chosen DX application—like Work Requests—right from your dashboard. It’s a clean, card-style layout that’s great for tracking, reviewing, and acting on records without jumping between screens. You can apply filters, check key details, and even kick off transitions or create new entries—all within the widget.

***

#### 2. What Does It Show?

This widget displays transaction records from the DX application (e.g., Work Request)  you select. Each record appears as a card showing useful info like: priority, creation time, created user, and stage. The top of the widget shows a configurable title, while the interface offers tools for creating new transactions, performing transitions, and filtering results.

Clicking the filter icon opens a popup that allows users to refine the displayed records using either **Basic** or **IQL-based** filtering. The configured filters like—_created user, assignee, priority, and date range_ appear in this popup.

***

#### 3. Where Does the Data Come From?

All data comes from DX Applications. You pick one app, and the widget pulls in its transactions. You can apply Filters to retrieve only relevant records based on user-defined conditions (like specific users or dates).

***

#### 4. Data Source Component Breakdown

<figure><img src="../../.gitbook/assets/1 - 2025-06-09T032536.927.png" alt=""><figcaption></figcaption></figure>

**Component 1: DX Application**\
Lets you select the DX application whose transactions should be displayed (_e.g., Work Request)_

**Component 2: Filter Query (IQL)**\
Allows you to enter advanced filtering logic using iviva Query Language (IQL). This is optional but can be used to apply more complex business rules for data retrieval.

***

#### 5. General Details Component Breakdown

<figure><img src="../../.gitbook/assets/1 - 2025-06-09T032829.905.png" alt=""><figcaption></figcaption></figure>

**Component 1: Title**\
Custom title shown at the top of the widget (e.g., _Work Request_)

**Component 2: Disable Filters**\
If selected, end-users will not be able to use any filters—the whole filtering feature gets disabled.

**Component 3: Show Filters in Popup**\
Displays the filters in a popup window instead of inline

**Component 4: Enable Create User Filter**\
Adds a filter option for the user who created the transaction

**Component 5: Enable Assignee User Filter**\
Adds a filter option for the transaction’s assigned user

**Component 6: Enable Priority Filter**\
Adds a filter for transaction's priority (e.g., High, Medium, Low)

**Component 7: Enable Create Date Filter**\
Adds a date range filter for the transaction creation date

**Component 8: Enable Perform Transition**\
Allows users to perform actions (e.g., _Closure, Approval_) right from each card

**Component 9: Enable Transaction Create**\
Adds a button to create a new transaction directly from the widget

**Component 10: Show Total Count**\
Displays the total number of transactions retrieved

***

#### 6. Search Card Configurations

<figure><img src="../../.gitbook/assets/1 - 2025-06-09T033111.898.png" alt=""><figcaption></figcaption></figure>

**Component 1: Card Layout Mode**\
Choose how the cards are visually styled. Options include **Default, Simple,** or **Alert styles**

**Component 2: Main Title Field**\
Select the primary field to display as the main heading of each card (optional)

**Component 3: Subtitle Fields**\
Choose additional fields to appear below the main title—such as _CreatedBy, Created Date, and Priority._ These appear in smaller text within the card.

**Component 4: User Priority Colour as Border Colour**\
Adds a coloured border around the card based on its priority level

**Component 5: User Priority Colour as Background**\
Uses the priority colour as the card's background colour for visual emphasis

**Component 6: Show Priority Chip**\
Displays a colour-coded label (chip) for the priority level (_e.g., HIGH, MEDIUM, LOW)_

**Component 7: Show Created User Details**\
Shows information about the user who created the transaction (_e.g., Admin User)_

**Component 8: Show Stage Chip**\
Displays a label showing the current stage of the transaction (_e.g., New, Closure_)

***

#### 7. Display Options

* **Responsive Layout:** The widget adapts to different screen sizes and displays neatly as a list of cards.
* **Transaction Count & Create Option:** A count badge at the top indicates the number of retrieved transactions, and a "Create" button allows adding new ones.
* **Filter Popup:** Click the filter icon in the top-right  to open a popup with both **Basic** and **IQL** filtering options.
  * _Basic mode_ supports dropdowns and date ranges
  * _IQL mode_ allows advanced text-based filters for power users
* **Real-Time Updates:** Changing filters dynamically refreshes the card list
* **Interactive Cards:** Cards show user-defined fields and allow quick actions like transitions—if enabled.

***

#### 8. Dashboard Visual Breakdown

<figure><img src="../../.gitbook/assets/1 - 2025-06-09T033605.781.png" alt=""><figcaption></figcaption></figure>

**Component 1: Widget Title**\
Displays the name of the selected DX application _(e.g., Work Request_)

**Component 2: Filter Popup**\
The popup contains both basic and advanced search options. It reflects all filters enabled during configuration (_e.g., Created User, Assignee, Priority, Date Range_). Switching between **Basic** and **IQL** lets users choose how they want to filter data.

**Component 3: Create Button**\
Allows users quickly create a new transaction—if enabled in configuration

**Component 4: Transaction Card**\
Each transaction appears as an individual **card** that visually summarises all the key details for quick understanding and action. Clicking a card redirects the user to the detailed page of the transaction. The card includes:

* A **coloured priority chip** (e.g., HIGH in red, MEDIUM in yellow, LOW in green) that immediately communicates the urgency of the transaction.
* The **transaction ID** as the main label for easy identification
* **User and date information** beneath the title, showing when the transaction was created and by whom, with associated icons.
* A **stage chip** on the right-hand side (e.g., Closure, New) that shows the current workflow stage of the transaction.\
  Additionally, **hover over the three dots next to the stage chip** to view available workflow transitions. Selecting one opens a **transition form in a popup**, allowing users to perform actions such as closing or reassigning the transaction directly from the widget. This makes updates fast and interactive—no need to leave the dashboard.
