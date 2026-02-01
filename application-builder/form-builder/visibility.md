# Visibility

The **Visibility** tab lets you show or hide fields based on specific conditions set by the form designer. This makes the form dynamic, showing fields only when they are relevant—for instance, based on other user inputs. This kind of logic makes the form easier to use by keeping it clean and focused—only the relevant fields show up.

<figure><img src="../../.gitbook/assets/image (92).png" alt=""><figcaption></figcaption></figure>

**Component 1 → Make This Field Hidden**\
Turn the **Make This Field Hidden** toggle on to keep the field permanently hidden—no matter what rules (expressions) or data values are in place. The field will not show up on the form at all, even if other visibility settings would normally display it.

**Component 2 → Visibility Expressions List**\
This area lists all the existing expressions that control when the field appears. Each expression is a logical condition—for example, “Problem Title Not Empty”—that checks the current form data. If any condition is true, the field shows up. If none are met—and the 'Hidden' toggle is off—the field stays hidden. To remove an expression, just click the trash-can icon next to it.

**Component 3 → Add Expressions**\
Click the **Add Expressions** button.

<figure><img src="../../.gitbook/assets/image (93).png" alt=""><figcaption></figcaption></figure>



**1→Make This Field Hidden**

**2 →Expressions Group Name**

* Before adding any conditions, you will need to name the group of expressions. Imagine it as a label for a set of rules that will be evaluated together. For example, 'Show-When-Priority-High' or 'Display-If-Approved.'&#x20;
* This is where you select the field that your condition will check. Once you have entered a group name, click the **Field** dropdown (marked as ③ in your screenshot) and choose any field in the form (e.g., _Problem Title, Location, Status_). Once you have selected a field , you will set:
  * **Comparison Operator** (_e.g., Equals, Not Empty, Contains)_
  * **Value** (if the operator requires a comparison against a specific value)
* In practice, here is what you do:
  1. Click the **Field** dropdown to see all available form fields.
  2. Choose the field you want to monitor.
  3. Set the condition (_e.g., Problem Title → Not Empty or Status → Equals Approved_).
  4. Click **+ Add** to add that condition to the current expression group.
* Once you save, the condition gets added to the **Visibility Expressions** list. If the selected field’s state matches your rule—like “Problem Title is not empty”, the target field will show up. If you have added multiple conditions, those conditions follow the group’s logic (you can choose whether **all** conditions **must be true** or **any** one is enough).

You can combine multiple expressions to create more advanced visibility logic—like "show certain section only when Field A is not empty or Field B equals ‘Approved'." This improves the user experience by showing only the fields that matter, based on real form data.
