# 👤 User

The **User field** allows you to select a system user from the list of registered users. This is commonly used for assigning users, capturing responsible parties, or recording who performed a certain action.

<figure><img src="../../../.gitbook/assets/New Project (2) (1).jpg" alt=""><figcaption></figcaption></figure>

> 🔸 What is a User Entity ?
>
> In iviva DX, a User is someone who can log in with valid credentials. Users represent real people such as staff, managers, or contractors—who interact with the system.
>
> * **Users belong to User Groups** (e.g., Admins, Supervisors, Technicians)
> * **User Groups have User Roles**
>   * Roles define what users can access and do in the system
> * **Roles determine Permissions**
>   * Permissions control which parts of the app a user can view or modify after logging in



#### 🪄  Default Value: Fill with Current User

This field type offers an additional smart default:

* **Option**: `Fill with Current User`
* **Purpose**: Automatically selects the **currently logged-in user**
* **Use Case**: Useful for audit fields like "Reported By", "Requested By", or "Created By"
* **Overrides**: Can be combined with conditional logic if needed
