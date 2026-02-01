---
description: >-
  The Update Transaction block allows users to update a DX transaction by
  providing the appropriate app key and required form data.
---

# Update Transaction

<figure><img src="../../.gitbook/assets/General Update Transaction.png" alt=""><figcaption><p> Update Transaction block</p></figcaption></figure>

> ### **Input Pins**

{% hint style="info" %}
#### The  Update Transaction block has multiple input pins.

You can provide individual pins corresponding to each search ID. For example, if the search ID of a text field is defined as 'Text', a value like 'ExampleTest' can be given and assigned to that specific field.
{% endhint %}

<details>

<summary>AppKey</summary>

This is the app key for a particular application.

Data Type : <mark style="color:orange;">Integer</mark>

```
Example  :  1
```

</details>

<details>

<summary>TransactionKey</summary>

Transaction Key for the updated transaction

Data Type : <mark style="color:orange;">Integer</mark>

```
Example  :  5
```

</details>





> ### **Output Pins**

<details>

<summary>AppKey</summary>

This is the app key for a particular application.

Data Type : <mark style="color:orange;">Integer</mark>

```
Example  :  1
```

</details>



<details>

<summary>TransactionKey</summary>

Transaction Key for the updated transaction

Data Type : <mark style="color:orange;">Integer</mark>

```
Example  :  5
```

</details>

<figure><img src="../../.gitbook/assets/General Update Transaction Lucy.png" alt=""><figcaption><p>Example: Using the Update Transaction block in a real application</p></figcaption></figure>
