# SLA Configuration

The **SLA (Service Level Agreement) Configuration** section is used to define **time-bound rules** for managing the flow of transactions across different **workflow milestones (stages)**. By configuring SLAs, users can specify how quickly specific stage transitions should happen, helping ensure accountability and timely progress.

This is particularly useful in workflows where stages mark critical milestones and timing affects performance tracking, escalation, or process optimisation.

<figure><img src="../../../.gitbook/assets/image (33).png" alt=""><figcaption></figcaption></figure>

**Component 1** → **SLA Label**

Displays the name of the SLA (_e.g., Respond, Review, or any custom label)_, identifying the time rule that has been applied.

**Component 2** → **Edit Button**

Click this button to open the SLA editing panel, where you can modify any configured SLA details.

**Component 3** → **Delete Button**

Click this button to remove the corresponding SLA from the configuration list.

**Component 4** → **Add SLA Panel**

Click the Add SLA button to open the Add SLA panel, where you can add a new SLA.

<figure><img src="../../../.gitbook/assets/image (35).png" alt=""><figcaption></figcaption></figure>



* **1 → SLA Name**\
  Used to add a descriptive name for the SLA rule. This name will be shown in the SLA table.
* **2 → Start Stage**\
  Select the workflow stage where the SLA timing begins.
* **3 → End Stage**\
  Select the workflow stage where the SLA timing ends.
* **4 → Include Non-Working Hours**\
  Select the **Include Non-Working Hours** check box to have the SLA timing count **all hours**, including non-working hours. This is ideal for time-sensitive processes that require round-the-clock tracking.
* **5 → Allow to Reset SLA on Workflow Loop Back**\
  Select the **Allow to Reset SLA on Workflow Loop Back** check box to reset SLA timing whenever the workflow returns to the start stage. This is particularly useful for workflows that involve **rework** or revision cycles.
* **6 → Exclude Stages**\
  Select the **Exclude Stages** check box to exclude specific stages from SLA tracking. This gives you more flexibility to define which time periods should or should not count.

**Component 5** → **Add Priority Panel**

SLAs can be tied to different priority levels to accommodate varying urgency or importance. Each priority can have its own timing thresholds. Click the Priority button to open the Add Priority panel.

<figure><img src="../../../.gitbook/assets/image (36).png" alt=""><figcaption></figcaption></figure>

* **1 → Priority Name**\
  The name of the priority level (_e.g., High, Medium, Low_).
* **2 → Priority Colour**\
  Assign a colour to each priority to make it visually distinct and easy to identify.
* **3 → Is Default**\
  Select the **Is Default** check box to mark the priority as the system default, which will be applied automatically unless another priority is selected.

**Component 6** → **Priority Label**

Displays all defined priorities along with their assigned colours (_e.g., High – Red, Medium – Yellow_). One priority will also be marked as 'Default.'

**Component 7** → **Time Duration Fields**

Time Duration fields allow you to define the **expected time limits** (in minutes) for each priority level. These durations determine how long a transaction can stay within the defined SLA path based on its assigned priority. You can enter different values for each priority to reflect urgency

For example, shorter times for 'High' priority and longer for 'Low' priority. These fields are editable directly within the grid, ensuring each task is tracked against its expected time.

**Component 8** → **Edit Button**

Click the edit button to modify the selected priority, including its name, colour, and default status.

**Component 9** → **Delete Button**

Click the delete button to remove the priority level entirely from the SLA configuration.
