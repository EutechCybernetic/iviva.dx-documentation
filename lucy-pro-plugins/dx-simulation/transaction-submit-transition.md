---
description: >-
  The Simulate Submit Transition block allows you to submit a specific
  transition within a DX transaction by providing the relevant App Key,
  Transaction Key, Transition ID, and any required form data.
---

# Transaction Submit Transition



<figure><img src="../../.gitbook/assets/SimulateSubmitTranstion.png.png" alt=""><figcaption><p> Simulate Submit Transition Block</p></figcaption></figure>

> ### **Input Pins**

{% hint style="info" %}
#### The Simulate Submit Transition Block has multiple input pins.

You can provide individual pins that match the search IDs of specific fields. For example, if a text field has the search ID Text, you can assign it a value like 'ExampleTest' and that value will be applied directly to that field.
{% endhint %}

<details>

<summary>AppKey</summary>

This is the app key for a particular application.

Data Type : <mark style="color:orange;">Integer</mark>

```
Example  :  14
```

</details>

<details>

<summary>TransactionKey</summary>

This is the transaction key for the transaction that is getting updated.

Data Type : <mark style="color:orange;">Integer</mark>

```
Example  :  112
```

</details>

<details>

<summary>TransitionID</summary>

The Transition ID lets you update the transaction’s stage.

Data Type : String

```
Example  :  TS_17303499864339ZKTI8QGMCV
```

</details>



> ### **Output Pins**

<details>

<summary>AppKey</summary>

This is the app key for a certain application.

Data Type : <mark style="color:orange;">Integer</mark>

```
Example  :  14
```

</details>

<details>

<summary>TransactionKey</summary>

This is the transaction key for the generated transaction.

Data Type : <mark style="color:orange;">Integer</mark>

```
Example  :  112
```

</details>

<figure><img src="../../.gitbook/assets/transactionSubmitTransitionLucy.png.png" alt=""><figcaption><p>Example: Using the Simulate Submit Transition block in a real application</p></figcaption></figure>

