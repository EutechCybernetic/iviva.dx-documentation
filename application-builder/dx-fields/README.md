# 🧰 DX Fields

## 🧩 Introduction to DX Fields in iviva.DX

In the **iviva.DX** no-code platform, **DX Fields** are the key components for building forms. These fields allow users to **capture, display,** and **process information** without writing a single line of code. Whether you are creating a form for tasks, transactions, or object records, DX Fields give you flexible building blocks to design intuitive and intelligent user interfaces.

<figure><img src="../../.gitbook/assets/New Project (1).jpg" alt=""><figcaption></figcaption></figure>

Each field is designed for a specific data type (text, date, number, object reference, etc.) and comes with configurable behaviours, validations, display settings, and integration support, allowing the platform to adapt to various business workflows.

***

## 📦 Available DX Field Types

The following DX Field types are available:

### 📝 Input Fields

* **Single Line Text** – Single-line text input
* **Multi-Line Text (Text Area)** – Multi-line text box
* **Rich Text** – Text input with formatting options (bold, lists, hyperlinks)
* **Number** – Numeric-only input

### ✅ Selection Controls

* **Static Dropdown** – A drop-down menu with one selectable option
* **Static Multiple Selection** – Used to choose multiple options from a static list
* **Short List** – A compact dropdown with limited visible options
* **Option Button Group** – Radio-button style choices
* **Button Group** – Multi-choice buttons that behave like toggles

### 🔘 Boolean Controls

* **Check Box** – Basic true/false check box
* **Toggle Switch** – Used to turn a setting on or off

### 🔗 Object References

* **Object Reference** – Link to a single object from another module (e.g., User, Asset)
* **Object Group** – Multiple object references grouped as one field
* **Transaction Reference** – References a transaction form or record

### 🌐 External and System Fields

* **Web Link Field** – Allows adding a single hyperlink
* **Web Link Group** – Stores multiple URLs or resource links
* **System Fields** – Auto-generated fields like _Created By, Modified Date_

### 📅 Date and Time Fields

* **Date** – Used to select a calendar date
* **Time** – Used to pick a time of day
* **Date Time** – Used to choose both date and time together

### 📱 Contact and Identity Fields

* **Email** – Enter email address with format validation
* **Phone** – Enter a phone number in a standardised format
* **Address** –Fill in a structured address with street, city, state, and other details

### 🖼️ Media and File Inputs

* **Image Picker** – Upload or select an image
* **File Selector** – Attach files or documents
* **Signature Pad** – Capture a digital signature

### 🎨 UI Style and Visual Pickers

* **Colour Picker** – Allows users to choose a colour using a palette or RGB/Hex
* **Icon Picker** – Select icons for labelling or design

### 📊 Tabular and Rating Inputs

* **Simple Table** – Enter data in a simple, easy-to-use table
* **Advanced Table** – Create a table with custom formulas, validations, and configurations
* **Rating** – Provide ratings visually using stars, numbers, or other scales

### 🗺️ Location and Team Inputs

* **Geo Map** – Pick a location on a map
* **Team Selector** – Assign users or teams based on roles

***



### ⚙️ Common Properties for All DX Field Types

In **iviva DX**, all field types includes a set of common configuration options. These settings control the **field’s behaviour, visibility, editability, style,** and **how it integrates** with backend systems such as APIs, filters, workflows, and data-binding engines.

> 💡 **Note:**
>
> * Both **Name** and **Search Index** must be **unique** and are essential for the correct functioning of form logic and system integration.

<figure><img src="../../.gitbook/assets/image (139).png" alt=""><figcaption></figcaption></figure>

***

#### 🏷️ Name

* **What it is:** The main identifier or label displayed to users
* **Required:** ✅ Yes
* **Purpose:** Helps users easily understand the field's purpose on the form
* **Notes:** This is the default label seen by users unless a  `Display Name` is provided.

***

#### 📝 Display Name

* **What it is:** A more descriptive or localised label for the field
* **Fallback:** If not set, the `Name` value is used automatically.
* **Use case:** Ideal for multilingual support or for a clearer, user-friendly labels
* **Note:** Useful in UI localisation and branding adjustments

***

#### 🔍 Search Index

* **What it is:** A unique, system-level key for referencing the field internally
* **Required:** ✅ Yes
* **Rules:**
  * Must be **globally unique** within the app
  * **No spaces or symbols** (use capitalise words)
* **Used in:**
  * API payloads
  * Filtering logic
  * Workflow rules
  * Data-binding operations
* **Impact:** Incorrect or missing Search Index may break backend logic or cause data issues.

***

#### ❗ Mandatory (Required Field)

* **What it is:** Specifies that the field must be filled before submitting the form
* **Effect:** The form blocks submission and shows an error if the field is left empty.
* **Use case:** For capturing important information such as Email, ID number, etc.

***

#### 🚫 Read-Only

* **What it is:** Prevents users from editing the field
* **Use case:** Useful for system-generated values, calculated fields, or audit data

***

#### 👁️ Hidden

* **What it is:** Hides the field from the form
* **Usage:** Can be set manually or triggered dynamically using **visibility rules**
* **Benefit:** Keeps forms clean by showing fields only when needed

***

#### 👁️ Visibility Conditions

* **What it does:** Shows or hides the field based on other field values, user actions, or form context
* **Example:** Shows a "State" dropdown only when "Country" is selected as "USA"
* **Benefit:** Enhances UX by keeping forms cleaner and context-aware

***

#### ✍️ Editability Conditions

* **What it does:** Controls when the field can be edited or locked, based on dynamic logic
* **Example:** Makes the “Discount” field editable only when the “Customer Type” is “Premium”
* **Benefit:** Ensures data integrity and enforces business logic directly in the UI

***

#### 🪄 Default Value

* **What it is:** The value automatically filled in when the form loads
* **Usage:** Can be a static string, a number, or a value bound dynamically via form context or user data
* **Benefit:** Saves user effort and aligns the form with preset logic or defaults

***

#### 💡 Placeholder

* **What it is:** Temporary hint text shown inside an empty field
* **Purpose:** Guides the user on what input is expected or in what format
* **Note:** Disappears when the user starts typing

***

#### ℹ️ Info (Tooltip)

* **What it is:** A small info icon that display extra guidance when hovered or clicked
* **Use case:** Explains the purpose of the field or expected input
* **Benefit:** Reduces confusion and input errors

***

#### 👤 Show Name

* **What it is:** Controls whether the field’s label (`Name`) is visible to users
* **When enabled:** The label appears above or beside the input
* **When disabled:** The label is hidden — useful for compact layouts or when context is already clear
* **Benefit:** Offers flexibility in form design

***

#### 🎨 Custom CSS Styling

Customise the field appearance to match your branding or layout needs using these options:

* **`inputClass`** – CSS class for the input element itself (e.g., _text box, dropdown_)
* **`wrapperClass`** – CSS class for the outer container of the field
* **`additionalStyles`** – Inline CSS or extra class names for detailed customisation
* **Use case:** Adjust padding, margins, colours, fonts, or any visual aspect
* **Benefit:** Makes forms blend in visually with your product’s design and branding

#### 🧵 `Enable for Text Search`

* **Purpose**: Enables **free-text search** application
* **Effect**: Field is included in global keyword searches in listings or reports
* **Use Case**: Useful for fields like _Text, TextArea, etc._

***

#### 🧩 `Enable in Filters`

* **Purpose**: Includes the field in the **structured filter panel**
* **Effect**: Users can apply exact or advanced filters using this field (_e.g., dropdowns, date pickers_)
* **Use Case**: Ideal for filtering records by status, category, date, or user-defined values
