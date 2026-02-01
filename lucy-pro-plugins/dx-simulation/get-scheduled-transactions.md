---
description: >-
  The Simulate Get Scheduled Transactions block returns all the scheduled
  transactions for a specific scheduler. To get the upcoming transactions,
  provide the scheduler key— that is all you need.
---

# Get Scheduled Transactions

<figure><img src="../../.gitbook/assets/GetScheduledTransactions (1).png" alt=""><figcaption><p>Simulate Get Scheduled Transactions Block</p></figcaption></figure>

<details>

<summary>SchedulerKey</summary>

Scheduler Key for the particular scheduler

Data Type : <mark style="color:orange;">Integer</mark>

```
Example  :  5
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

Allows you to specify which record to start retrieving data: 0 begins with the first record, 1 skips the first record

Data Type : <mark style="color:orange;">Integer</mark>

```
Example  :  0
```

</details>

> ### **Output Pins**

<details>

<summary>Scheduled Transactions</summary>

Scheduled Transactions of the provided scheduler

&#x20;Type : List

```
Example  : [ { "HasParent": "False", "Transactions": "[ { "App": { "DisplayText": "TestAPI", "Value": "35" }, "HasParent": false, "TargetStartDate": "2024-11-07T17:30:00Z", "RecurrenceType": "Daily", "Pattern": 1, "Checklists": [ { "Checklist": { "DisplayText": "Checklist Name", "Value": "48" }, "ServiceItems": [ { "displayText": "1000", "objectType": "Asset", "value": "3" } ] } ] } ]" }, { "HasParent": "False", "Transactions": "[ { "App": { "DisplayText": "TestAPI", "Value": "35" }, "HasParent": false, "TargetStartDate": "2024-11-08T17:30:00Z", "RecurrenceType": "Daily", "Pattern": 1, "Checklists": [ { "Checklist": { "DisplayText": "Checklist Name", "Value": "48" }, "ServiceItems": [ { "displayText": "1000", "objectType": "Asset", "value": "3" } ] } ] } ]" }, { "HasParent": "False", "Transactions": "[ { "App": { "DisplayText": "TestAPI", "Value": "35" }, "HasParent": false, "TargetStartDate": "2024-11-09T17:30:00Z", "RecurrenceType": "Daily", "Pattern": 1, "Checklists": [ { "Checklist": { "DisplayText": "Checklist Name", "Value": "48" }, "ServiceItems": [ { "displayText": "1000", "objectType": "Asset", "value": "3" } ] } ] } ]" }, { "HasParent": "False", "Transactions": "[ { "App": { "DisplayText": "TestAPI", "Value": "35" }, "HasParent": false, "TargetStartDate": "2024-11-10T17:30:00Z", "RecurrenceType": "Daily", "Pattern": 1, "Checklists": [ { "Checklist": { "DisplayText": "Checklist Name", "Value": "48" }, "ServiceItems": [ { "displayText": "1000", "objectType": "Asset", "value": "3" } ] } ] } ]" }, { "HasParent": "False", "Transactions": "[ { "App": { "DisplayText": "TestAPI", "Value": "35" }, "HasParent": false, "TargetStartDate": "2024-11-11T17:30:00Z", "RecurrenceType": "Daily", "Pattern": 1, "Checklists": [ { "Checklist": { "DisplayText": "Checklist Name", "Value": "48" }, "ServiceItems": [ { "displayText": "1000", "objectType": "Asset", "value": "3" } ] } ] } ]" } ]
```

</details>

<figure><img src="../../.gitbook/assets/Get Scheduled Transactions Lucy.png" alt=""><figcaption><p>Example: Using the Simulate Get Scheduled Transactions Block in a real application</p></figcaption></figure>
