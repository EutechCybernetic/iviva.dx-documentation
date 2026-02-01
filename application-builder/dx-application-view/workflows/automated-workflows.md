# Automated Workflows

The **Automated Workflow** section allows users to set up conditional automation rules that trigger during workflow execution. This helps to reduce manual effort and ensure consistent task handling based on defined conditions.&#x20;

Each automation consists of a set of conditions and one or more resulting actions, that run automatically when the conditions are met. This is useful for scenarios like auto-assigning tasks, sending notifications, or creating linked records (_e.g., CWOs_) when specific criteria are satisfied.

<figure><img src="../../../.gitbook/assets/1 (33) (1).png" alt=""><figcaption></figcaption></figure>

**Component 1 → Configure Automated Workflow**\
Click the **Configure Automated Workflow** link to open the configuration panel, where you can create a new automated workflow. Users can define the condition(s) and the corresponding automated action(s) to be executed.

<figure><img src="../../../.gitbook/assets/1 (32) (1).png" alt=""><figcaption></figcaption></figure>

**1 → Enable Automation**\
A toggle to turn the automation on or off. When **Enable Automation** toggle is on, the automation rule runs once all conditions are met.

**2 → Automation Title**\
Enter a unique and meaningful title for the automation. This helps in identifying the automation rule easily in the list view.

**3 → Automation Description**\
**Automation Description** is an optional field where users can describe the purpose or logic of the automation rule for future reference.

**4 → Trigger When**\
Used to select the event or system trigger that will initiate the automation rule. For example, when a transaction is created.

**5 → Add Conditions**\
Click the **Add Conditions** link to specify logical conditions that must be satisfied for the automation to run. Multiple conditions can be added to create complex rules.

**6 → Add Actions**\
Defines what the system should do once the conditions are met. Examples include sending emails, updating fields, or creating linked records.

**Component 2 → Edit Button**\
Allows users to edit the existing automation rule, including the conditions or actions applied.

**Component 3 → Delete Button**\
Permanently removes the selected automation from the app.

**Component 4 → Duplicate Button**\
Creates a copy of an existing automation. This is useful for quickly replicating similar rules with minor changes.

**Component 5 → Condition Count**\
Displays the number of **conditions** configured for the automation rule.

**Component 6 → Action Count**\
Indicates the number of **actions** defined in the automation.

**Component 7 → Automation Status**\
Shows whether the automation is currently **enabled** or **disabled**.

* **Enabled**: The rule is active and will execute when its conditions are met.
* **Disabled**: The rule exists but will not run until explicitly enabled.\
  This status helps users manage which automations are live and which are still in testing or under configuration.

By defining automated workflows, users can streamline app behaviour, ensure timely actions, and enforce operational consistency without manual intervention.
