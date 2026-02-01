# User Roles

**User Roles**

The **User Roles** section allows administrators to define how different roles interact with forms, fields, transactions, and visibility settings throughout the application. Once a user group is assigned a role through the **Access Rights** panel on the **App Details Page**, permissions configured here will apply automatically. This is crucial for ensuring that each user only sees or interacts with data relevant to their responsibilities.

<figure><img src="../../.gitbook/assets/image (54).png" alt=""><figcaption></figcaption></figure>

**Component 1 → Add Role**\
Click the + button to open Add User Role panel, allowing users to create a new user role (_e.g., Admin, Operator)_. Then each role can be configured with different access permissions.

<figure><img src="../../.gitbook/assets/image (57).png" alt=""><figcaption></figcaption></figure>

**Component 2 → Edit Role**\
Allows users to modify a user role's name and description.

**Component 3 → Delete Role**\
Removes the user role entirely from the application.

**Component 4 → Form Visibility Access by User Role**\
Defines which **forms** the selected user role can view or interact with. Forms include the initial form and all transition forms (_e.g., New Work Request, Rework, Acknowledge Work Request_).

**Component 5 → Fields Visibility Access by User Role**\
Specifies which **fields** are visible to the user role within each form. This helps control access to sensitive or irrelevant data.

<figure><img src="../../.gitbook/assets/image (55).png" alt=""><figcaption></figcaption></figure>

**Component 6 → Editable Fields in Details**\
Defines which fields the role can **edit** in the transaction detail view (_e.g., updating the problem title, service category, or asset)._ Non-editable fields will appear read-only.

<figure><img src="../../.gitbook/assets/image (56).png" alt=""><figcaption></figcaption></figure>

**Component 7 → Transactions**\
Allows to configure the permissions such as the ability to delete one's own or others' transactions.

**Component 8 → Enable Tabs in Details**\
Controls which **tabs** (_e.g.,  SLA, Checklist, Activity History)_ are visible in the transaction details panel for the user role.

**Component 9 → Actions**\
Grants the role access to action-based function, such as launching a workflow popup.

**Component 10 → Enable Search Page Actions**\
Determines which search functionalities are available to the selected role. Options include:

* **Enable Basic Search**
* **Enable IQL Search**

**Component 11 → Scope Filter Query**\
Allows administrators to define a custom filter using an **IQL query** to limit the data each user role can access.
