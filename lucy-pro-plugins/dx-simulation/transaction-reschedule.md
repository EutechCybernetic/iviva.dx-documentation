---
description: >-
  The Simulate Transaction Reschedule block allows you to reschedule a
  transaction's schedule details by providing the App Key and the Transaction
  Key.
---

# Transaction Reschedule

<figure><img src="../../.gitbook/assets/Simulate Transactio Reschedule.png" alt=""><figcaption><p>Simulate Transaction Reschedule Block</p></figcaption></figure>

> ### **Input Pins**

{% hint style="info" %}
#### The Simulate Transaction Reschedule block has multiple input pins.

You can update the following pins: `TargetStartDate` and `TargetEndDate` (DateTime).


{% endhint %}

<details>

<summary>AppKey</summary>

This is the App Key for a particular application.

Data Type : <mark style="color:orange;">Integer</mark>

```
Example  :  14
```

</details>

<details>

<summary>TransactionKey</summary>

This is the Transaction Key of the transaction you want to reschedule.

Data Type : <mark style="color:orange;">Integer</mark>

```
Example  :  112
```

</details>





> ### **Output Pins**

<details>

<summary>AppKey</summary>

This is the App Key for a particular application.

Data Type : <mark style="color:orange;">Integer</mark>

```
Example  :  14
```

</details>

<details>

<summary>TransactionKey</summary>

This is the Transaction Key for the rescheduled transaction.

Data Type : <mark style="color:orange;">Integer</mark>

```
Example  :  112
```

</details>

<figure><img src="../../.gitbook/assets/Transaction Reschedule Lucy.png" alt=""><figcaption><p>Example: Using the Simulate Transaction Reschedule Block in a real application</p></figcaption></figure>
