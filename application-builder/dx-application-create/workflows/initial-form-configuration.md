# Initial Form Configuration

The Initial Form Configuration allows you to design and build the starting form for your workflow. This form captures the essential information that initiates the application process and serves as the foundation for all subsequent actions. The configuration is visual and interactive, giving you full control to customise both the layout and behavior of your form.&#x20;

<figure><img src="../../../.gitbook/assets/1 (10) (1).png" alt=""><figcaption></figcaption></figure>

**Component 1 - Form Preview**\
This shows a live preview of how your form will appear to users. As you add or update fields, the preview updates in real time, letting you see the final version instantly. It offers a clear visual reference to help structure and test your form layout before deployment.

**Component 2 - Form Configuration Panel**\
This panel displays all the fields included in your form. You can customise fields to suit your needs — set default values, control field visibility, make fields editable or read-only, and apply filters to refine drop-down menus or related data inputs. This ensures your form works intelligently and captures the right information at the right time.

**Component 3 - Fields Pallet**\
This section contains a variety of form fields that you can drag and drop into your form. The fields are grouped into two main categories:

* **System Fields**: These are predefined fields connected to system-level entities. Examples include:
  * User
  * User Group
  * Location
  * Asset
  * Cost Center\
    System fields pull real-time values from your application’s underlying system data. They are useful for assigning users, tagging locations, or managing cost allocations.
* **Custom Fields**: These fields allow you to capture user-defined input. Examples include:
  * Single Line Text
  * Email
  * Address
  * Date/Time
  * Attachment\
    Custom fields are flexible and can be used to collect any type of specific input not available through system fields.

**Component 4 - Form Settings Panel**\
Click the settings icon to open a panel where you can configure how your form behaves.&#x20;

<figure><img src="../../../.gitbook/assets/1 (11) (1).png" alt=""><figcaption></figcaption></figure>

**1 → Form Name**\
The internal name used to identify the form within the application.

**2 → Form Description**\
A short explanation of the form’s purpose, helping users understand the type of data being collected.

**3 → Form Submit Action**\
This determines what happens when the form is submitted:

* **Create Object:** The system automatically calls the relevant service and creates a transaction using the form data.
* **Lucy Model Action:** Lets you run a custom or third-party action. You can choose an existing Lucy model and action or create a new one tailored to your needs.

**4 → Make Public and Share**\
Select the **Make Public and Share** check box to make the form publicly accessible so users without login credentials can submit it.

**5 → Remove Cancel Button**\
Select the **Remove Cancel Button** check box to hide the cancel button on the form, which is useful if you want to prevent users from accidentally discarding the form.

**6 →** **Submit Button Text**\
Allows you to customise the label on the submit button _(e.g., Send Request or Confirm Submission)._

**7 → Execute Lucy Model Action on Form Onload**\
Defines what happens automatically when the form loads. Select the **Execute Lucy Model Action on Form Onload** check box to trigger a Lucy model action as soon as the form appears.&#x20;

This is useful for tasks such as auto-populating fields, fetching third-party data, or applying business rules immediately. Just like the submit action, users can select a predefined Lucy model or create a new one to meet their specific needs.

Together, these options provide you everything needed to build a powerful, flexible, and responsive entry form for your application.&#x20;

Once your configuration is complete, click **Next** to continue.
