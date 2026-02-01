---
description: >-
  The Simulate Update Checklist block allows you to update a checklist. You need
  to provide the Checklist Key to specify which checklist to update.
---

# Update Checklist

<figure><img src="../../.gitbook/assets/Simulate Update Checklist.png" alt=""><figcaption><p>Simulate Update Checklist Block</p></figcaption></figure>

> ### **Input Pins**

{% hint style="info" %}
#### The Simulate Update Checklist block has multiple input pins

You can update the following pins: `ChecklistName`(String),`TotalDuration`(Integer), `CountDurationFromTasks`(Integer), `RequiredIndividualTaskCompletion`(Boolean), and `Tasks`(Dictionary List).


{% endhint %}

<details>

<summary>ChecklistKey</summary>

This is the checklist key of the checklist to be updated.

Data Type : <mark style="color:orange;">Integer</mark>

```
Example  :  49
```

</details>





> ### **Output Pins**

<details>

<summary>Checklist Details</summary>

Displays the status of the checklist after it has been updated

Data Type : <mark style="color:orange;">Dictionary</mark>

```
Example  :  { "ChecklistKey": "53", "ObjectKey": "53", "Status": "Updated" }
```

</details>

<figure><img src="../../.gitbook/assets/Simulate Update Checklist Lucy.png" alt=""><figcaption><p>Example of using the Simulate Update Checklist Block in a real application</p></figcaption></figure>
