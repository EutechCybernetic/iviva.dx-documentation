# Create Scheduler

Clicking the **Create** button opens a popup form where users can define a new scheduler. By filling in the required details such as the scheduler name, description, and recurrence settings, checklist details, service items, and schedule actions, users can successfully create and save a new scheduled task.

### Schedule Details

<figure><img src="../../.gitbook/assets/image (83).png" alt=""><figcaption></figcaption></figure>

**Component 1:** The **Schedule Name** input field allows users to assign a unique and identifiable title to the new schedule being created. This is a required field for saving the scheduler.

**Component 2:** The **Schedule Description** text area enables users to provide additional context or notes about the schedule, helping clarify its purpose or include any relevant details for future reference.



### Recurrence Details

<figure><img src="../../.gitbook/assets/1 (67).png" alt=""><figcaption></figcaption></figure>

**Component 1:** The **Recurrence Pattern** section allows users to define how often the scheduler should run—Daily, Weekly, Monthly, or Yearly—along with the interval between executions (e.g., every 1 day).

**Component 2:** The **Range of Recurrence** section lets users specify when the schedule begins and whether it has an end. Users can choose between **No End Date**, ending after a specific number of occurrences, or ending by a specific date.

**Component 3:** The **Start Time** field allows users to set the exact time of day when the scheduled task should trigger on its scheduled dates.

**Component 4:** The **Generate Before (days)** field determines how many days in advance the scheduler should generate the transaction before the actual scheduled date, allowing pre-processing or early preparation.



### Checklist Details

<figure><img src="../../.gitbook/assets/image (84).png" alt=""><figcaption></figcaption></figure>

**Component 1:** The **Default Checklist** dropdown allows users to select the primary checklist that will be used for the scheduler. This checklist contains the standard set of tasks to be followed.

**Component 2:** The **Override Checklists for Advance Scheduling** toggle enables users to specify an alternative checklist for special cases or specific scheduled dates, overriding the default checklist when necessary.

**Component 3:** The **Recurrence Pattern** dropdown allows users to define the specific day(s), month(s), or year(s) when the override should apply—based on the overall recurrence settings configured earlier.

**Component 4:** The **Override Checklist With** dropdown provides the option to select an alternative checklist that will replace the default checklist for the specified recurrence pattern.



### Other Details

<figure><img src="../../.gitbook/assets/image (86).png" alt=""><figcaption></figcaption></figure>

**Component 1:** The **Add New** link under **Service Items** allows users to insert specific service-related tasks into the schedule. These service items define the work or actions to be performed during the scheduled execution.

**Component 2:** The **Use a Single Checklist for All Items of Service** checkbox enables users to apply one common checklist across all service items instead of assigning individual checklists to each.

**Component 3:** The **Create Transaction From** dropdown allows users to select the DX application or transaction form that the scheduler should use to generate scheduled transactions.

**Component 4:** The **Create a Single Transaction for All Items of Service** checkbox lets users consolidate multiple service items into a single transaction, simplifying execution and tracking.

**Component 5:** The **Enable Parent Transaction** checkbox allows users to link all generated transactions under a single parent, providing a hierarchical structure that’s useful for organizing complex or multi-step processes.

**Component 6:** The **Parent DX Application** dropdown appears when **Parent Transaction** is enabled. It allows users to select the parent application under which the scheduled transactions will be grouped.
