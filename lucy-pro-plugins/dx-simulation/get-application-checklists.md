---
description: >-
  The Simulate Get Application Checklists block returns all checklists linked to
  a specific checklist key used in an application. You can provide both the app
  key and the checklist key to retrieve them.
---

# Get Application Checklists

<figure><img src="../../.gitbook/assets/GetApplicationCheckLists.png.png" alt=""><figcaption><p> Simulate Get Application Checklists block</p></figcaption></figure>

> ### **Input Pins**

<details>

<summary>AppKey</summary>

This is the app key for a particular application.

Data Type : <mark style="color:orange;">Integer</mark>

```
Example  :  35
```

</details>

<details>

<summary>ChecklistKey</summary>

The checklist key associated with the checklist

Data Type : <mark style="color:orange;">Integer</mark>

```
Example  :  49
```

</details>

<details>

<summary>max</summary>

Allows you to specify how many checklists you want to return

Data Type : <mark style="color:orange;">Integer</mark>

```
Example  :  20
```

</details>

<details>

<summary>last</summary>

Allows you to specify the starting point for data retrieval. Use 0 to start at the first record, 1 skips it.

Data Type : <mark style="color:orange;">Integer</mark>

```
Example  :  0
```

</details>

<details>

<summary>q</summary>

Allows to filter by checklist id or checklist name, like search filter

Data Type : String

```
Example  :  API Checklist
```

</details>

<details>

<summary>ObjectKey</summary>

Allows you to filter checklists by the object key

Data Type : <mark style="color:orange;">Integer</mark>

```
Example  :  1
```

</details>

<details>

<summary>ObjectType</summary>

Allows you to filter checklists by their object type

Data Type : String

```
Example  :  Asset
```

</details>

> ### **Output Pins**

<details>

<summary>Application Checklists</summary>

The checklists in the DX application



Data Type : List

```
Example  : [ { "CountDurationFromTasks": "1", "Tasks": "[ { "AllowImageProofing": false, "IsCompleted": false, "Attachments": [], "Comments": [], "Duration": 6, "AllowComments": false, "AllowToSkipMandatoryWithComment": false, "TaskName": "Text", "TaskValue": null, "FieldType": "Text", "IsMandatory": false } ]", "RequiredIndividualTaskCompletion": "0", "ChecklistID": "CLT_1726208864368OXXB3P1X4HG", "row_id": "1", "ChecklistKey": "48", "totalcount": "1", "Completed": "0", "TotalDuration": "6", "TransactionKey": "7", "TargetEndDate": "", "TargetStartDate": "", "IsSystemGenerated": "0", "SchedulerKey": "", "AppKey": "35", "ChecklistMapKey": "1", "ChecklistName": "Checklist Name", "Description": "", "Objects": "[]" } ]
```

</details>

<details>

<summary>__totalcount__</summary>

Total number of checklists



Data Type : Integer

```
Example  : 10
```

</details>

<figure><img src="../../.gitbook/assets/GetApplicationChecklistLucy.png.png" alt=""><figcaption><p>Example: Using the Simulate Get Application Checklists block in a real application</p></figcaption></figure>
