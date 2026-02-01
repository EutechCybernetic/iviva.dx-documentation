---
description: >-
  The Simulate Get Create Form block gives all the fields in the create form for
  a specific app using the App Key. It helps users see what fields are available
  and get a quick overview of the data.
---

# Get Transaction Create Form

<figure><img src="../../.gitbook/assets/SimulateGetCreateForm.png.png" alt=""><figcaption><p>Simulate Get Create Form Block</p></figcaption></figure>

<details>

<summary>AppKey</summary>

This is the app key for a particular application.

Data Type : <mark style="color:orange;">Integer</mark>

```
Example  :  35
```

</details>

> ### **Output Pins**

<details>

<summary>CreateForm</summary>

The app’s Create form



Data Type : Dictionary

```
Example  :  { "Result": "{ "Name": "test", "ID": "FM_1730349986433CFFLY5W0I", "FieldTemplates": { "Text": { "FieldType": "Text", "ValueType": "String", "Example": "Example Text" } } }" }
```

</details>

<figure><img src="../../.gitbook/assets/GetTransactionCreateFormLucy.png" alt=""><figcaption><p>Example: Using the Simulate Get Create Form Block in a real application</p></figcaption></figure>
