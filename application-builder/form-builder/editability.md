# Editability

The **Editability** tab controls whether a field can be edited in the form—either always or only under certain conditions. This lets form designers to control when and how users can input or modify values—useful for scenarios where certain fields should only be editable at specific stages or by specific roles.

<figure><img src="../../.gitbook/assets/image (94).png" alt=""><figcaption></figcaption></figure>

**Component 1 → Make This Field Read-only**\
Turn the **Make This Field Read-only** toggle on to lock the field—users will not be able to edit it, no matter its visibility or default settings. If the toggle is off, the field stays editable unless a rule says otherwise.

**Component 2 → Editability Expressions**\
Click the **Add Expressions** link to set up conditional logic that dynamically switch the field to read-only mode. In the **Editability Expressions** box, you can define one or more rules that lock the field whenever those conditions are met.

* **Expression Group Name** (not shown in this cropped view). This is the label for your rule set (e.g., '_Lock-When-Location-Filled'_).
* Below the group name, each line follows the format 'When \[Field] \[Operator] \[Value/State].' For example, 'When Location Not Empty' means the field becomes read-only as soon as the **Location** field has any value.

**Component 3 → Add Expressions**\
Clicking **Add Expressions** opens the editor where you create new rules. In the editor you will choose:

* **Field**–Pick any existing form field (e.g., _Location_).
* **Condition**– Select a condition such as _Not Empty, Equals, Contains._
* **Expected Value**–Enter a specific value if the operator requires it (_e.g., a specific text, or number_).\
  After defining a condition, click **+ Add** to append it. After saving, any field that matches these conditions will automatically become read-only.

By combining the toggle and expressions, you can either blanket-lock a field (by toggling it on) or lock it only under precise circumstances (via expressions)—ensuring users can edit it only when appropriate.
