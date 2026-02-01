# View Configuration

The **View Configuratio**n section lets developers and administrators control the behaviour and appearance of the transaction detail view. It allows them to configure how record details are displayed, organised, and interacted with by end users.

This section is divided into three main areas: detail view behaviour, custom section layout, and feature-specific toggles.

<figure><img src="../../../.gitbook/assets/image (44).png" alt=""><figcaption></figcaption></figure>

**Component 1 → Override Submission with Lucy Model Action**

Enable the **Override Submission with Lucy Model Action** check box to override the submission button with a predefined action model, allowing custom workflows or logic to run when a submission occurs.

#### **Component 2 → Enable Public Access Without Login**

Select the **Enable Public Access Without Login** check box to allow users to access the transaction detail view without logging in. This is useful for publicly shareable forms or reports.

#### **Component 3 → Enable Transaction QR Code**

Choose the **Enable Transaction QR Code** check box to display a QR code on the detail page. Scanning the QR code with a mobile device opens the transaction detail view directly.

#### **Component 4 → Enable Transition Action Bar**

Replaces the traditional hover-based transition menu in the detail view header. Instead, transitions are displayed as clearly labeled clickable buttons in a dedicated bar below the header. Clicking a transition opens the corresponding transition form. This bar can also include a customizable **Update** button, which appears when field values have been modified but not yet saved. It helps users apply or discard changes easily, reducing the risk of unsaved edits and improving usability.

<figure><img src="../../../.gitbook/assets/1 (59).png" alt=""><figcaption></figcaption></figure>

#### **Component 5 → Scroll to Last Details Section on Refresh**

Select the **Scroll to Last Details Section on Refresh** check box to automatically scroll to the last open detail section when the page refreshes, enhancing user convenience and continuity.

#### **Component 6 → Details Submit Button Text**

Used to customise the label on the form submission button _(e.g., Update, Save Changes_) to clearly reflect the action.

<figure><img src="../../../.gitbook/assets/image (45).png" alt=""><figcaption></figcaption></figure>

**Component 7 → Create Section Button**

Click the **Create Section** button to allow administrators to define new custom sections in the detail view layout. This opens the _Add New Section_ panel, providing precise control over how and when each section is displayed.

<figure><img src="../../../.gitbook/assets/image (43).png" alt=""><figcaption></figcaption></figure>

**1 → Section Name**

Used to enter the display name for the section (_e.g., Asset Details, Additional Info_).

**2 → Visible Section Based on Field Value**

Allows conditional visibility of this section based on the value of another field in the form.

This option defines the **triggering logic** for section visibility:

* **Availability**: The system checks if the selected field(s) are _present_ or _filled_. This is useful when the section should appear simply based on whether a field has been shown or contains a value.
* **Value**: The system evaluates the _actual value_ of the selected field(s). The section will appear only if the field matches the specific criteria.

**4 → Successive Field Consideration**

Used to choose **how multiple fields are evaluated together:**

* **All**: Show the section only if all selected fields meet the condition.
* **Any**: Show the section if at least one selected field meets the condition.

(Select one option using the radio buttons.)

**5 → Fields Dropdown**

Allows the user to select which field(s) will control the visibility logic.

**6 → Use as a Successive Field**

Select the **Use as a Successive Field** check box to mark the selected field as a **required condition** in successive logic. Use it when the section’s display depends on this field being present or meeting a specific value.

<figure><img src="../../../.gitbook/assets/1 (64).png" alt=""><figcaption></figcaption></figure>

**Component 8 → Enable Checklist Section**

Choose the **Enable Checklist Section** check box to display the checklist panel on the transaction detail page. When enabled, users can view and manage itemised checklists.

#### **Component 9 → Enable Schedule Section**

Select the **Enable Schedule Section** check box to display the Scheduling panel on the transaction detail page. Also, it allows users to define which fields represent the start and end dates for scheduled events _(e.g., Scheduled Start Date)._

**Component 10 → Enable Conversation Section**

Select the **Enable Conversation Section** check box to display the Conversation section on the transaction detail page, supporting internal communication and collaboration.

**Component 11 → Enable SLA Section**

Select the **Enable SLA Section** check box to activate the SLA  panel on the transaction detail page, showing the transaction's SLA progress or status. SLA calculation can be based on the following:

* Assigned Users' Working Hours
* Organization Working Hours
* Location Working Hours

These options allow flexible SLA computation strategies to match operational needs.

The **View Configuration** section significantly enhances the user experience by enabling a highly customisable and informative transaction detail layout. Using these settings, applications can better match business processes and user expectations.
