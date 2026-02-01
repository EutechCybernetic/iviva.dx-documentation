# DX Datalist

#### 1. Introduction

<figure><img src="../../.gitbook/assets/web and mobile7.png" alt=""><figcaption></figcaption></figure>

The **DX Datalist Widget** is a versatile visual tool used to show data entries as cards. It allows users to browse, search, filter, and interact with individual records in a DX application. This widget is especially useful for summarising entries such as locations, tasks, users, or other records that fit well in a structured, scrollable list.

***

#### 2. What Does It Show?

The widget displays a dynamic list of items from your chosen data source. Each item appears as a **card** that can include titles, descriptions, subtitles, and even custom icons. You can customise the card layout and content to suit your needs. Each card can also include clickable actions—like opening a form, triggering a service, or jumping to a URL.

***

#### 3. Where Does the Data Come From?

The widget supports the following data sources:

* **API** – Pulls data from an external API
* **iviva Service** – Uses backend services to retrieve internal data
* **Lucy** – Connects to low-code platform data models

To configure these data sources, please refer to the respective sections on [API](./#id-1.2.-api) Setup, [iviva Service](./#id-1.3.-iviva-service) Setup, or [Lucy ](./#id-1.4.-lucy)Integration. Parameter configuration for the respective sections is also mentioned in the respective links.

Once configured, the data will automatically show up as cards in the widget.

***

#### 4. Data Source Component Breakdown

<figure><img src="../../.gitbook/assets/1 - 2025-06-10T202217.566.png" alt=""><figcaption></figcaption></figure>

**Component 1: Use Filter Form**\
Enables filtering for the datalist widget using a custom-built form.

**Component 2: Edit Form**\
Opens a form builder popup. Inside the builder:

* Add a static dropdown
* Rename the **Search Index** and **Label** to the filter name (e.g., _Location Type_)
* Set matching dropdown values
* In **Value Bind**, set `dx.get_value_from` to match the filter field name

**Component 3: Show Filters in Popup**\
If enabled, filters show up in a popup. If disabled, filters stay visible on the widget.

{% hint style="info" %}
For details on setting up data sources (API, iviva Service, and Lucy) , check the links mentioned earlier.
{% endhint %}

***

#### 5. General Details Component Breakdown

<figure><img src="../../.gitbook/assets/1 - 2025-06-10T202438.534.png" alt=""><figcaption></figcaption></figure>

**Component 1: Show Title Bar**\
The **Show Title Bar** toggle controls whether the widget header with title and icon is visible. Turn it on to make them visible.

**Component 2: Title**\
Set the title that appears at the top of the widget

**Component 3: Subtitle**\
Add an optional subtitle to give extra context

**Component 4: Icon**\
Choose an icon to match the widget’s theme

***

#### 6. Card Configuration

<figure><img src="../../.gitbook/assets/1 - 2025-06-10T203717.881.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/1 - 2025-06-10T204257.775.png" alt=""><figcaption></figcaption></figure>

**Component 1: Preview**\
Shows a live preview of the card layout based on current configuration

**Component 2: Card Layout Mode**\
Select a card style such as _Default, Simple, Alert, Count, Image, or Table._

**Component 3: Main Title Card**\
Sets the main field shown on each card. Click the edit(pencil icon) to open the next component.

**Component 4: Edit Field**\
Lets you:

* Rename the field title
* Select which field to show
* Set how the field should appear _(e.g., text)._

**Component 5: Description**\
The **Description** works like the Main Title—customisable via the same edit popup.

**Component 6: Subtitles**

This toggle shows or hides the **Subtitle** section below the main title and description.\
When it is on, you can add extra fields to enrich the card—like Location Type, Status, and more.

**Component 7: Add New Subtitle**

The **Add New Subtitle** panel on the right allows you to **add a new subtitle**. Each entry includes:

* **Field Title** – Label shown on the card
* **Field** – The actual data field to display
* **Icon** – Optional icon to visually represent the field
* **Type** – Defines how the data should be formatted or interpreted (_e.g., text, number, date)_
* **Add button** – Click to add the configured subtitle to the card preview

**Component 8: Subtitle Configuration**

The **Subtitle Configuration** allows you to fine-tune how subtitles look:

* **Show Titles** toggle – Shows or hides the field titles in the subtitle area
* **Display as ROW / COLUMN** – Controls whether subtitles appear horizontally (Row) or vertically (Column)
* **Display as BLOCK / INLINE** – Adjust spacing and alignment for each subtitle field

This gives fine-grained control over how the subtitle content appears visually.

**Component 9: Enable Card On Click Action**

This toggle controls whether clicking on a card **triggers an action**—like opening a form, calling a service, or navigating somewhere.\
When enabled, the 'Edit On Click Action link' becomes functional.

**Component 10: Edit On Click Action**\
Opens a [side panel ](dx-datalist.md#side-panel-edit-on-click-action-component-wise-explanation)with further configurations options

**Component 11: Action Buttons (For the Card)**

This section defines **action buttons that appear on each card.**

Each button is **rendered directly on the card,** allowing users to perform quick actions like updating or deleting the item shown. Details for setting this up are covered in the [Action Configuration ](dx-datalist.md#id-7.-action-configuration)section.

***

#### Side Panel: Edit On Click Action (Component-Wise Explanation)

<figure><img src="../../.gitbook/assets/1 - 2025-06-10T205339.595.png" alt=""><figcaption></figcaption></figure>

***

**Action Type Tabs**\
Choose how the action should work:

* **API** – Integrate with an external API
* **Iviva Service** – Use a built-in backend service for tasks like updating or retrieving data
* **Lucy** – Trigger logic defined in Lucy (a low-code automation tool)
* **URL** – Redirect the user to a specified web link

In **parameter configuration**, always set the **source as `List`** and specify the **field value from the card’s data** that you want to send to the action. This applies to **all action types** — API, iviva Service, Lucy, and URL.

**Why Always Use “List”?**

* Using 'List' ensures the parameter dynamically pulls the value from the selected card.
* It is the most accurate way to **contextually bind** the action to the exact item clicked — whether it is invoking an API, triggering a Lucy model, updating via iviva service, or navigating to a URL.

#### URL Configuration (in 'Edit On Click Action' or 'Add action')

Unlike API, iviva Service, or Lucy, the **URL configuration** lets you **redirect the user to another page or app** by forming a dynamic link.

* **URL Template**: This is where you define the target URL. You can insert dynamic values using placeholders like `#{LocationKey}`.
* **Parameters**: Set parameters using:
  * **Type: List** (to fetch from the card data)
  * **Field**: Specify which field's value to inject into the URL placeholder .

This option works **differently from other types**:

* It **does not invoke a backend action or service**
* It simply **navigates the user to another page**—optionally using card data to customise the destination.



(Refer to the configuration guides for [API](./#id-1.2.-api),[ iviva Service](./#id-1.3.-iviva-service), and [Lucy](./#id-1.4.-lucy) for setup help.)

***

**Component 1: Use DX Form**\
Turn this on if you want the action to show a form when triggered—so users can input or edit data before it runs.

***

**Component 2: Edit Form**\
Click the **Edit Form** button to open the form builder. You can use this form to **pass data to the service** instead of using the parameters section directly. Here is how:

> **How to Set Up the Edit Form for Passing Data**

1. Add fields that match the required service parameters (e.g., _to update a location name, add a field for_ `FullName`)
2. For each field:
   * Set the **Search Index** and **Label** to the expected parameter name (e.g., `FullName`).
   * In the **Value Bind** section, ensure `dx.get_value_from` is set to the same parameter name (e.g., `FullName` ).

This ensures the form passes the right values to the action when submitted.

***

**Component 3: Success Message**\
You can customise a confirmation message to display when the action completes successfully (e.g., _Location updated successfully)_.

***

**Component 4: Refresh List on Success**\
When enabled, the Datalist widget refreshes automatically after the action runs—so users see the latest data right away.

***

#### 7. Action Configuration

<figure><img src="../../.gitbook/assets/1 - 2025-06-10T210313.632.png" alt=""><figcaption></figcaption></figure>

This section allows you to configure global action buttons that appear at the **top of the DX Datalist Widget**, separate from the cards. These actions let users trigger services—like _creating records_—outside the individual cards.

***

#### **Component 1: Add New Action (+)**

Click the **plus button** in the top-right to configure and add a new action button.\
This opens the same **side panel** as described under the **Edit On Click Action** component, where you can:

* Set the action type (API, iviva Service, Lucy, URL)
* Define the service or endpoint
* Add parameters or configure a form (if needed)

> The interface and configuration process are identical to what was covered above.

***

#### **Component 2: List of Configured Actions**

Displays all the action buttons that have been added so far. Each action is shown as a **card** containing:

* The **button title** (e.g., `Create`)
* The **action type** (e.g., `Service`)

Each card shows a quick summary of how the action is set up.

***

#### **Component 3: Edit Action**

The **pencil icon** on each action card allows you to update the configuration of that specific action.\
Click the icon to reopen the configuration side panel, where you can:

* Modify parameters
* Change form behaviour
* Update the success message or icon

***

#### **Component 4: Delete Action**

Use the trash bin icon to remove an action button that is no longer relevant to the widget.

***

#### Side Panel: Add or Edit Action (Component-wise Explanation)

<figure><img src="../../.gitbook/assets/1 - 2025-06-10T211138.527.png" alt=""><figcaption></figcaption></figure>

**Component 1: Button Title**\
Set the text label for the button (e.g., _Update_)

**Component 2: Icon**\
Pick an icon for the button

**Component 3: Icon Only**\
Enable this to show just the icon—no text

**Component 4: Button Type**\
Choose the style for the button

***

You can configure the action using one of the following:

* **API**
* **iviva Service**
* **Lucy**
* **URL**

In each case:

* Specify the target service or URL
* Use the form builder to map input values if required
* Ensure the field’s value bind is set correctly to match what the endpoint expects

***

**Component 5: Use DX Form**\
Enable this to show a form when the action is triggered—so users can input or edit data before it runs.

***

**Component 6: Edit Form**\
Click to open a form builder. You can use this form to **pass data to the service** instead of using the parameters section directly. Here's how:

> 🛠 **How to Set Up the Edit Form for Passing Data:**

1. Add fields that match the required service parameters (e.g., To create a location name, add a field for `FullName`).
2. For each field:
   * Set the **Search Index** and **Label** to the expected parameter name (e.g., `FullName`)
   * In the **Value Bind** section, ensure `dx.get_value_from` is set to the same parameter name (e.g., `FullName` ).

This ensures the form passes the correct values to the action when submitted.

***

**Component 7: Success Message**\
You can customise a confirmation message to display when the action completes successfully (e.g., _Location created successfully)_.

***

**Component 8: Refresh List on Success**\
When enabled, the Datalist widget refreshes automatically after the action runs—so users see the latest data right away.

***

#### 8. Display Options

The widget offers various display options depending on the chosen card layout:

* **Show or Hide Title Bar** with icon and subtitle
* **Different Card Modes** (Simple, Default, Image, Alert, etc.)
* **Row or Column Layout** for subtitles
* **Inline or Block** display for card content
* **Card-level Actions** – visible on each card
* **Widget-level Actions** – shown at the top of the widget

***

#### 9. Dashboard Visual Breakdown

<figure><img src="../../.gitbook/assets/1 - 2025-06-10T211745.810.png" alt=""><figcaption></figcaption></figure>

#### **Component 1: Widget Title**

* Displays the title of the widget
* '_Location_' in this example.
* Helps users understand the type of data the card is showing

***

#### **Component 2: Action Configurations Action Buttons (Create)**

* Adds new actions such as **Create**, **Add**, or other global functions
* These are configured from the **Action Buttons** section in the **Action Configuration**
* The button label reflects the configuration (e.g., _Create_)

***

#### **Component 3: Filter**

* Opens the **filter configuration popup** if popup mode is enabled
* If not enabled, a dropdown appears instead
* Used to narrow down the card results based on filter criteria

***

#### **Component 4: Card**

* Represents a single item record in the list (e.g., a specific location)
* Layout and fields shown are determined by your **card configuration**

***

#### **Component 5: Card Actions Configured**

* Configurable icons (like the pencil icon for **edit**) show up here
* Actions such as **Update**, **Redirect**, or custom logic can be triggered when the card is clicked
* Defined in the **Action Buttons** section in **Card Configuration**

***

#### **Component 6: Main Title**

* The primary field shown at the top of the card
* Example: “KANDY”, “ITC”, etc.
* Configured via the **Main Title** setting in the Card layout builder

***

#### **Component 7: Description**

* A secondary field shown just below the main title
* Example: “1” or “2” in your cards
* Configured in the **Description** field section

***

#### **Component 8: Subtitle**

* Additional metadata like “LocationType: Site” or “LocationType: Building”
* Multiple subtitles can be added
* Shown inline or in block layout depending on subtitle settings
