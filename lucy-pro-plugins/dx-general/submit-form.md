---
description: The Submit Form block allows saving form model data within a transition.
---

# Submit Form



<figure><img src="../../.gitbook/assets/General Submit Form.png" alt=""><figcaption><p>Submit Form block</p></figcaption></figure>

> ### **Input Pins**

<details>

<summary>AppKey</summary>

This is the app key for a particular application.

Data Type : <mark style="color:orange;">Integer</mark>

```
Example  :  36
```

</details>

<details>

<summary>TransactionKey</summary>

Transaction Key for the generated transaction

Data Type : <mark style="color:orange;">Integer</mark>

```
Example  :  19
```

</details>

<details>

<summary>FormModel</summary>

Form Model with required details for saving the transaction

Data Type : <mark style="color:orange;">Dictionary</mark>

```
Example  :  { "name": "Transaction details has been updated", "isInitialForm": false, "id": "FM_C2E3E187-105A-4A16-84D0-6D6DC89BEB99", "description": "", "fields": [ { "type": "DateTime", "id": "DAT_1726208774790OHEX2KS03DN", "searchIndex": "Date1", "datatype": "DATETIME", "status": "New", "name": "New Date Time Field", "placeholder": "", "isReadonly": null, "isMandatory": null, "isHidden": null, "column": "Field5", "editability": null, "visibility": null, "value": null }, { "type": "DateTime", "id": "DAT_1726208775811QOH2SZ28WY", "searchIndex": "Date2", "datatype": "DATETIME", "status": "New", "name": "New Date Time Field (1)", "placeholder": "", "isReadonly": null, "isMandatory": null, "isHidden": null, "column": "Field6", "editability": null, "visibility": null, "value": null }, { "type": "Text", "id": "TX_1726725204268GT70WAKA5IJ", "searchIndex": "NewTextField", "datatype": "STRING", "placeholder": "", "status": "New", "name": "New Text Field", "isReadonly": null, "isMandatory": null, "isHidden": null, "editability": null, "visibility": null, "column": "Field7", "value": "" }, { "type": "SystemDropdown", "id": "DL_1729486382622C8T5AK67KNU", "searchIndex": "Organization", "datatype": "JSON", "status": "New", "ivivaObjectType": "Organization", "service": "DXCommon:OrganizationAll", "app": "IvivaDX", "name": "Organization", "keyField": "OrganizationKey", "displayField": "OrganizationName", "supportedFilters": [ "Organization" ], "isReadonly": null, "isMandatory": null, "isHidden": null, "editability": null, "visibility": null, "column": "Field2", "value": null }, { "type": "SystemDropdown", "id": "DL_1731312133132CI7IZUL70IQ", "searchIndex": "User", "datatype": "JSON", "status": "New", "ivivaObjectType": "User", "service": "DXCommon:UserAll", "app": "IvivaDX", "name": "User", "keyField": "UserKey", "displayField": "FullName", "subTextField": "UserGroupID", "supportedFilters": [ "Site", "User Group", "User Type", "User" ], "isReadonly": null, "isMandatory": null, "isHidden": null, "editability": null, "visibility": null, "column": "Field8", "value": null }, { "type": "SimpleTable", "id": "STB_17313925357700CF48GVFUZP6", "searchIndex": "NewSimpleTable", "datatype": "ARRAY", "headings": [ "Column One", "Column Two", "Column Three" ], "status": "New", "name": "New Simple Table", "isReadonly": null, "isMandatory": null, "isHidden": null, "editability": null, "visibility": null, "column": "Field9" }, { "type": "ButtonGroup", "id": "BTNG_1731920220178WU0C3GTBKRA", "searchIndex": "NewButtonGroup", "datatype": "STRING", "status": "New", "choices": [ "Button One", "Button Two", "Button Three" ], "name": "New Button Group", "isReadonly": null, "isMandatory": null, "isHidden": null, "editability": null, "visibility": null, "value": "Button Two" } ], "metaFields": [ { "id": "st_stage", "name": "Stage", "datatype": "STRING", "type": "StaticDropdown", "isReadonly": true, "isHidden": true, "showName": false, "column": "Stage", "status": "Existing", "searchIndex": "Stage", "value": "In-Progress", "choices": [ "Open", "In-Progress", "Co
```

</details>





> ### **Output Pins**

<details>

<summary>AppKey</summary>

This is the app key for a particular application.

Data Type : <mark style="color:orange;">Integer</mark>

```
Example  :  36
```

</details>

<details>

<summary>TransactionKey</summary>

Transaction Key for the generated transaction

Data Type : <mark style="color:orange;">Integer</mark>

```
Example  :  19
```

</details>

<figure><img src="../../.gitbook/assets/General Submit Form Lucy.png" alt=""><figcaption><p>Example: Using the Submit Form block in a real application</p></figcaption></figure>
