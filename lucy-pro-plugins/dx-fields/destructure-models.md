---
description: The Destructure Models block is used to decompose any JSON model.
---

# Destructure Models

<figure><img src="../../.gitbook/assets/Destructure Models.png" alt=""><figcaption><p>Destructure Models block</p></figcaption></figure>

> ### **Input Pins**

<details>

<summary>JSON</summary>

Model you want to break down

Data Type : <mark style="color:orange;">Dictionary</mark>

```
Example  :  { "Id": "TS_17303499864339ZKTI8QGMCV", "Label": "Start Work", "FromStage": { "name": "Open", "isActive": true }, "ToStage": { "name": "In-Progress", "isActive": true }, "FieldTemplates": { "Text": { "FieldType": "Text", "ValueType": "String", "Example": "Example Text" } } }
```

</details>





> ### **Output Pins**

{% hint style="info" %}
#### The Destructure Models block has multiple output pins.

You can give Attributes of JSON model as output pins.
{% endhint %}

<details>

<summary>AllOutput</summary>

The original model without any decomposition

Data Type : <mark style="color:orange;">Dictionary</mark>

```
Example  :  { "Id": "TS_17303499864339ZKTI8QGMCV", "Label": "Start Work", "FromStage": { "name": "Open", "isActive": true }, "ToStage": { "name": "In-Progress", "isActive": true }, "FieldTemplates": { "Text": { "FieldType": "Text", "ValueType": "String", "Example": "Example Text" } } }
```

</details>

<figure><img src="../../.gitbook/assets/Destructure Models Lucy.png" alt=""><figcaption><p>Example: Using the Destructure Models block in a real application</p></figcaption></figure>
