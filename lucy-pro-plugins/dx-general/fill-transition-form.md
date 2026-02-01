---
description: >-
  The Fill Transition Form block allows users to retrieve the transition model
  of a transaction by providing the app key, transaction key and transition ID.
---

# Fill Transition Form

<figure><img src="../../.gitbook/assets/General Fill Transition Form.png" alt=""><figcaption><p>Fill Transition Form block</p></figcaption></figure>

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

<summary>TransitionID</summary>

Transition ID for the generated transaction

Data Type : <mark style="color:orange;">String</mark>

```
Example  : "TS_17262087134770EHXB921O9JK"
```

</details>





> ### **Output Pins**

<details>

<summary>TransitionModel</summary>

Transition model for the specified transition ID

Data Type : <mark style="color:orange;">Dictionary</mark>

```
Example  : { "id": "TS_17262087134770EHXB921O9JK", "lable": "Start Work", "formModel": { "id": "FM_17262087134778Z3QOJ837CG", "name": "Start Work", "fields": [ { "type": "Text", "id": "TX_1726725204268GT70WAKA5IJ", "searchIndex": "NewTextField", "datatype": "STRING", "placeholder": "", "status": "New", "name": "New Text Field", "isReadonly": null, "isMandatory": null, "isHidden": null, "editability": null, "visibility": null, "column": "Field7", "value": "" }, { "type": "SystemDropdown", "id": "DL_1729486382622C8T5AK67KNU", "searchIndex": "Organization", "datatype": "JSON", "status": "New", "ivivaObjectType": "Organization", "service": "DXCommon:OrganizationAll", "app": "IvivaDX", "name": "Organization", "keyField": "OrganizationKey", "displayField": "OrganizationName", "supportedFilters": [ "Organization" ], "isReadonly": null, "isMandatory": null, "isHidden": null, "editability": null, "visibility": null, "column": "Field2", "value": null }, { "type": "SystemDropdown", "id": "DL_1731312133132CI7IZUL70IQ", "searchIndex": "User", "datatype": "JSON", "status": "New", "ivivaObjectType": "User", "service": "DXCommon:UserAll", "app": "IvivaDX", "name": "User", "keyField": "UserKey", "displayField": "FullName", "subTextField": "UserGroupID", "supportedFilters": [ "Site", "User Group", "User Type", "User" ], "isReadonly": null, "isMandatory": null, "isHidden": null, "editability": null, "visibility": null, "column": "Field8", "value": null }, { "type": "SimpleTable", "id": "STB_17313925357700CF48GVFUZP6", "searchIndex": "NewSimpleTable", "datatype": "ARRAY", "headings": [ "Column One", "Column Two", "Column Three" ], "status": "New", "name": "New Simple Table", "defaultValue": "[["a","b","c"],["d","e","f"],["g","h","i"]]", "isReadonly": null, "isMandatory": null, "isHidden": null, "editability": null, "visibility": null, "column": "Field9", "value": "[["a","b","c"],["d","e","f"],["g","h","i"]]" }, { "type": "ButtonGroup", "id": "BTNG_1731920220178WU0C3GTBKRA", "searchIndex": "NewButtonGroup", "datatype": "STRING", "status": "New", "choices": [ "Button One", "Button Two", "Button Three" ], "name": "New Button Group", "value": "" } ], "submit": { "action": { "Value": 1, "DisplayText": "Default Transition" } }, "linkInfo": { "enable": false }, "metaFields": [ { "id": "st_stage", "name": "Stage", "datatype": "STRING", "type": "StaticDropdown", "isReadonly": true, "isHidden": true, "showName": false, "column": "Stage", "status": "Existing", "searchIndex": "Stage", "value": "Open", "choices": [ "Open", "In-Progress", "Completed", "Closed" ] } ], "removeCancelButton": false, "removeSaveButton": false, "onLoadEvents": { "enable": true, "lucyModel": { "DisplayText": "DXDocument", "Value": "22" }, "lucyAction": { "DisplayText": "TestAPI", "Value": "TestAPI" } } }, "toStage": { "name": "In-Progress", "isActive": true }, "fromStage": { "name": "Open", "isActive": true } }
```

</details>

<figure><img src="../../.gitbook/assets/General Fill Transition Form Lucy.png" alt=""><figcaption><p>Example: Using the Fill Transition Form block in a real application</p></figcaption></figure>
