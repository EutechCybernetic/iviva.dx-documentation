# Transitions

The **Transitions** section allows you to define how your workflow moves from one stage to another, creating a clear and logical flow of actions within your application. This step is essential for ensuring tasks progress smoothly and the correct forms are shown at each stage.

<div data-full-width="false"><figure><img src="../../../.gitbook/assets/image (29).png" alt=""><figcaption></figcaption></figure></div>

**Component 1 - Workflow Diagram**

Displays a visual representation of how stages are connected through transitions. It helps users understand the flow of actions from one stage to another.

**Component 2 - Transition List**

Shows all configured transitions in a list format. Each row includes key details such as the transition name, source stage, destination stage, and the form associated with the transition.

**Component 3 - Transition Label**

Displays the name of the transition, such as 'Start Work' or 'Close Work.' This label represents the action performed during the transition.

**Component 4 - From Stage**

Indicates the starting point of the transition. This is the stage the transaction is currently in before the transition occurs.

**Component 5 - To Stage**

Shows the destination stage that the transaction will move to once the transition is executed.

**Component 6 - Add Transition**

This panel is used to define the behavior of a transition between two stages in the workflow. You can specify transition’s name, starting and ending stages, and which form the user sees when the transition is triggered.

<figure><img src="../../../.gitbook/assets/image (31).png" alt=""><figcaption></figcaption></figure>

* **1 → Transition Label**\
  This is the name or label of the transition. It represents the action performed (_e.g., Start Work or Submit for Approval_) and will be visible to users.
* **2 → From**\
  Specifies the starting stage of the transition. The transition will only be available when the transaction is in this stage.
* **3 → To**\
  Defines the destination stage the transaction moves to after the transition is triggered.
* **4 → Transition Form**\
  Associates a form with the transition. This form is shown to the user during the transition, allowing them to provide required information.
* **5 → New Form**\
  If you do not want to use an existing form, you can create a new one. Click the **New Form** link to open the form builder so you can design a custom form specific to the transition.
* **6 → Make Public and Share**\
  Select the **Make Public and Share check box** to make the transition form accessible via a public URL and QR code. This is useful for external users (such as vendors or clients) to submit information without logging in to the system.

**Component 7 - Edit Button**

<figure><img src="../../../.gitbook/assets/image (32).png" alt=""><figcaption></figcaption></figure>

Opens the edit panel where you can update transition details such as the label, from/to stages, and the form.

**Component 8 - Delete Button**

Removes the selected transition from the workflow permanently.

**Component 9 → Search Bar**

This search bar helps you quickly locate specific transitions by name. It is useful when managing workflows with multiple transitions, allowing you to filter and find the one you need without scrolling manually.

Transitions are the connecting threads of your workflow, ensuring each stage is actionable and the app knows what should happen next. This setup lets you create well-structured, rule-based flows that align with your process requirements.
