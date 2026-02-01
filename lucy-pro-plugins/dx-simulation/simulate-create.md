---
description: >-
  The Simulate Create block allows to create a DX transaction by passing in the
  right App Key and form data.
---

# Simulate Create

<figure><img src="../../.gitbook/assets/Simulate Create Checklist.png" alt=""><figcaption><p>Simulate Create Block</p></figcaption></figure>

> ### **Input Pins**

{% hint style="info" %}
#### The Simulate Create block has multiple input pins.

You can provide individual pins for each search ID. For example, if a text field has the search ID ‘Text’, you can assign it a value like ‘ExampleTest’, and it will be applied to that specific field.


{% endhint %}

<details>

<summary>AppKey</summary>

This is the app key for a particular application.

Data Type : <mark style="color:orange;">Integer</mark>

```
Example  :  1
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

This is the Transaction Key of the generated transaction.

Data Type : <mark style="color:orange;">Integer</mark>

```
Example  :  5
```

</details>

<figure><img src="../../.gitbook/assets/Simulate Create Lucy.png" alt=""><figcaption><p>Example of using the Simulate Create Block in a real application</p></figcaption></figure>
