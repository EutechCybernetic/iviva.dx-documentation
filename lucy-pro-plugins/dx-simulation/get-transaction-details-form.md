# Get Transaction Details Form

The Simulate Get Details Form block provides a list of fields in a transaction detail page by using the App Key and Transaction Key. It helps users track which fields are active at the current stage of the transaction.

<figure><img src="../../.gitbook/assets/SimulateGetDetailsForm.png.png" alt=""><figcaption></figcaption></figure>

<details>

<summary>AppKey</summary>

This is the app key for a particular application.

Data Type : <mark style="color:orange;">Integer</mark>

```
Example  :  35
```

</details>

<details>

<summary>TransactionKey</summary>

The Transaction Key of the required transaction

Data Type : <mark style="color:orange;">Integer</mark>

```
Example  :  6
```

</details>

> ### **Output Pins**

<details>

<summary>DetailsForm</summary>

Details form of the given transaction



Data Type : Dictionary

```
Example  : { "Result": "{ "Name": "Transaction details has been updated", "ID": "FM_435970DF-B3DB-402B-9B73-EC4E37467920", "FieldTemplates": { "Text": { "FieldType": "Text", "ValueType": "String", "Example": "Example Text" }, "TextNew": { "FieldType": "Text", "ValueType": "String", "Example": "Example Text" } } }" }
```

</details>

<figure><img src="../../.gitbook/assets/GetDetailsForm.png.png" alt=""><figcaption><p>Example: Using the Simulate Get Details Form block in a real application</p></figcaption></figure>
