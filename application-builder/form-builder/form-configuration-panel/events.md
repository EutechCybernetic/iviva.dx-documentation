# Events

The **Events** tab lets form designers to assign actions that respond automatically when the field’s value changes. This supports real-time workflows, advanced behaviours, and contextual data handling based on how users interact with the form.

<figure><img src="../../../.gitbook/assets/image (96).png" alt=""><figcaption></figcaption></figure>

**Component 1 → Override Submission with Lucy Model Action**&#x20;

Select the **Override Submission with Lucy Model Action** check box to override the standard saving process for the selected field. Instead of submitting normally, the updated value is intercepted and sent directly to a "Lucy Model" action.

By enabling this, any change to the field instantly starts your custom Lucy Model workflow, granting you full control over how and when the data is permanently saved.

**Component 1 → Enable Search for Options**

* Turn the **Enable Search for Options** toggle on to let end users type and search within the dropdown or lookup list, rather than scrolling through all available entries.
* When turned off, the field functions as a basic dropdown without an inline search box.

**Component 2 → Static Filters**

* Use this area to restrict the list of selectable options to a fixed set of values at design phase.
* **Filter Type** dropdown: Use the 'Filter Type' dropdown to choose from predefined filter categories. Once selected, that filter is always active, limiting the available options to whatever criteria the chosen filter type enforces.
* This ensures that, for example, only records meeting your organisation's business rules will appear in the field's selection list.

**Component 3 → Dynamic Filters**

* Set up runtime filters that depend on another field’s current value.
* **Filter By** dropdown: Select a “parent” field on the form whose value dynamically limits the lookup list.
* After selecting the parent field, click **Add** to lock in that relationship. During the runtime, any change to the parent field updates the lookup list to show only the items related to the parent field's current value.
