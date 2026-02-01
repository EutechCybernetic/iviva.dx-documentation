---
description: >-
  The Create Transaction block lets you create a DX transaction by providing the
  appropriate App Key and required field data.
---

# Create Transaction

<figure><img src="../../.gitbook/assets/General Create Transaction.png" alt=""><figcaption><p> Create Transaction block</p></figcaption></figure>

> ### **Input Pins**

<details>

<summary>AppKey  </summary>

This is the app key for the particular application.

Data Type : <mark style="color:orange;">Integer</mark>

```
Example  :  1
```

</details>

<details>

<summary>FormModel</summary>

The Primary Key of the transaction that needs updating

Data Type : <mark style="color:orange;">DIctionary</mark>

```
Example  :  { "name":"Transaction details has been updated", "isInitialForm":false, "id":"FM_E6F062FE-E3EE-424E-B0AC-6D3516B5CA72", "description":"", "fields":[ { "type":"DateTime", "id":"DAT_1726208774790OHEX2KS03DN", "searchIndex":"Date1", "datatype":"DATETIME", "status":"New", "name":"New Date Time Field", "placeholder":"", "isReadonly":null, "isMandatory":null, "isHidden":null, "column":"Field5", "editability":null, "visibility":null, "value":"2024-11-20T18:30:00Z" }, { "type":"DateTime", "id":"DAT_1726208775811QOH2SZ28WY", "searchIndex":"Date2", "datatype":"DATETIME", "status":"New", "name":"New Date Time Field (1)", "placeholder":"", "isReadonly":null, "isMandatory":null, "isHidden":null, "column":"Field6", "editability":null, "visibility":null, "value":null } ], "metaFields":[ { "id":"st_stage", "name":"Stage", "datatype":"STRING", "type":"StaticDropdown", "isReadonly":true, "isHidden":true, "showName":false, "column":"Stage", "status":"Existing", "searchIndex":"Stage", "value":"Open", "choices":[ "Open", "In-Progress", "Completed", "Closed" ] } ] }
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

The Transaction Key for the generated transaction

Data Type : <mark style="color:orange;">Integer</mark>

```
Example  :  112
```

</details>

<figure><img src="../../.gitbook/assets/General Create Transaction Lucy.png" alt=""><figcaption><p>Example: Using the Create Transaction block in a real application</p></figcaption></figure>
