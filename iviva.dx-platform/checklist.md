---
description: 'Stay Organized: Easily Manage and Track Tasks with the Checklist'
icon: list-check
---

# Checklist

The **Checklist** feature in the application allows users to keep track of important tasks, steps, or items within the application. It provides a simple and effective way to ensure nothing is missed by offering an organised list of actions, items, or to-dos that need to be completed.

### Key Features:

* **Search**: Easily search through your checklists to quickly find a specific checklist.
* **Task Management**: Add, edit, and remove items from your checklist.
* **Edit and Delete**: Modify or delete any checklist as needed.
* **Progress Tracking**: Mark tasks as completed to visually track your progress.

You can access the **Checklist** by clicking on the **Settings** icon located in the top-right corner of the [DX composer dashboard](../application-builder/dx-composer-dashboard.md) interface. Once you click the icon, a menu will appear where you can select **Checklist** to view and manage your tasks.

When the page opens, you will see a list of checklists along with other available options.

<figure><img src="../.gitbook/assets/1 (61).png" alt=""><figcaption><p>Checklist Page</p></figcaption></figure>

* **Component 1**: The **Search bar** is used to filter checklists by name. This helps users quickly locate a specific checklist without scrolling through the entire list, improving efficiency when working with larger datasets.
* **Component 2**: The **Create** button allows users to initiate the creation of a new checklist. Clicking it opens a popup where checklist details can be entered and saved.
* **Component 3**: The **Checklist display section** shows all existing checklists available to the user. Each checklist entry includes key information such as the name, duration, task count, and available actions.
* **Component 4**: The **Edit icon** allows users to modify an existing checklist including its name, duration, tasks, or other checklist configurations.
* **Component 5**: The **Delete icon** is used to permanently remove a checklist. A confirmation prompt may appear to prevent accidental deletions.
* **Component 6**: The **name of the checklist** serves as its main identifier. Clicking the name may redirect users to view or manage the tasks associated with that checklist.
* **Component 7**: Indicates the **estimated duration** required to complete the checklist. This helps users understand the time commitment for each checklist at a glance.
* **Component 8**: Displays the **number of tasks** included in the checklist. This gives users a quick overview of the checklist’s size and complexity.
* **Component 9**: The **Description field** (if provided), offers additional context or notes about the checklist's purpose or scope. This helps users understand its intent or any special instructions related to the checklist.

### Create New Checklist

<figure><img src="../.gitbook/assets/1 (63).png" alt=""><figcaption><p>Checklist Configuration</p></figcaption></figure>

* **Component 1**: **Checklist Name (Mandatory)**\
  Enter the name of the checklist. This is a required field and must be filled in before creating a checklist.
* **Component 2**: **Description (Optional)**\
  Enter an optional description to provide additional context or details about the checklist. This helps explain its purpose or any specific instructions.
* **Component 3**: **Count Duration from Task List**\
  When this checkbox is selected, the total duration of the checklist will be automatically calculated by summing the individual durations of each task added. When enabled, the **Total Duration** field becomes read-only and cannot be manually edited.
* **Component 4**: **Total Duration (Minutes)**\
  If the **Count Duration from Task List** checkbox is not selected, users can manually enter the total duration for the checklist here. This field becomes editable only when the duration is not being calculated from tasks.
* **Component 5**: **Required Tasks to Complete Individually**\
  When checked, this option ensures that each task within the checklist must be completed for the checklist to be marked as complete. It enforces strict task-by-task completion.
* **Component 6**: **Add Task**\
  Click this option to manually add custom tasks to the checklist. You will be guided through entering task names, durations, and other related fields (explained further below).
* **Component 7**: **From Existing Checklists**\
  Click this option to import tasks from previously created checklists. A panel will open showing a list of existing checklists and a search bar, allowing users to select and import tasks into the current checklist easily.
* **Component 8**: **Create Button**\
  Once all required fields are filled and at least one task is added, click this button to finalize and create the checklist. Note that **Checklist Name**, **Total Duration**, and at least one task are mandatory to proceed.

### Add Task

<figure><img src="../.gitbook/assets/1 (65).png" alt=""><figcaption><p>Add Task </p></figcaption></figure>

* **Component 1**: **Task Name (Mandatory)**\
  Enter the name of the task. This is a required field and must be filled in before adding the task to the checklist.
* **Component 2**: **Info (Optional)**\
  Provides an optional description or additional information about the task. This can include context, instructions, or any relevant details related to the task.
* **Component 3**: **Duration (Minutes) (Mandatory)**\
  Enter the estimated time (in minutes) required to complete this task. This field is required and contributes to the checklist's total duration if the option to count duration from the task list is enabled.
* **Component 4**: **Allow Comments**\
  When selected, users completing the task can add comments. This is useful for providing feedback, status updates, or additional notes during the task completion.
* **Component 5**: **Allow Image Proofing**\
  When selected, users are allowed (or required) to upload images as proof of task completion. This feature is especially useful for visual confirmation, especially in inspections, fieldwork, or documentation-heavy processes.
* **Component 6**: **Field Type (Mandatory)**\
  Select the type of input or response expected for this task (e.g., text, checkbox, dropdown). This defines how users will interact with and complete the task. It is a required field and must be selected to proceed.
* **Component 7**: **Mandatory**\
  When selected, this task becomes a required field for the checklist, meaning it must be completed before the checklist can be marked as done.
* **Component 8**: **Predefined Values**\
  If the selected field type supports predefined input (such as text, number, dropdown, checkbox, or radio options), you can specify a set of default values here. These predefined values act as suggested or default inputs that appear when the checklist is in use.
