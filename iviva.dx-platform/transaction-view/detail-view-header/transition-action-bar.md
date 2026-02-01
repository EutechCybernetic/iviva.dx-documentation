---
icon: diagram-successor
---

# Transition Action Bar

This page builds on the standard **Detail View Header**. In this enhanced view, the header still displays the **current stage**, but hovering over it no longer shows the available transitions. There is also an option to completely hide the current stage name if desired.

Instead, the **Transition Action Bar** below presents the available transitions as separate clickable buttons. Selecting any transition button opens the corresponding transition form.

The Transition Action Bar can also include an **Update** button (or a custom-labeled button based on configuration). When enabled, this button appears if changes are made to fields on the details page that have not yet been saved. It allows users to save updates or discard changes easily, helping prevent forgotten unsaved edits and improving the overall user experience.

<figure><img src="../../../.gitbook/assets/1 (34).png" alt=""><figcaption><p>Transaction Record with Transition Action Bar</p></figcaption></figure>

* **Section 1 : Transition Buttons**\
  Displays available transitions as individual buttons (e.g., Acknowledge, Cancel), allowing users to quickly select and initiate the desired workflow action.
* **Section 2 : Default/Recommended Transition**\
  Highlights the default or recommended transition for the current stage—often referred to as the "happy path." This transition is visually emphasized with an icon to prompt user action.
* **Section 3 : Guidance Message**\
  Shows a custom guidance message configured for the transition. In this example, it mirrors the transition name, but it can be customised to provide specific instructions or context.
* **Section 4 : Transition Icon**\
  Displays a configurable icon associated with the transition, helping visually communicate the nature or purpose of the action. Icons can be customized during application setup.

<figure><img src="../../../.gitbook/assets/1 (28).png" alt=""><figcaption><p>Update button appears for saving or discarding unsaved changes</p></figcaption></figure>

