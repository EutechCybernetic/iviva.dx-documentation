---
description: >-
  The Execute Service block lets users execute a service by providing the app
  name, model name, service call name, and any required parameters.
---

# Execute Service

<figure><img src="../../.gitbook/assets/General Execute Service.png" alt=""><figcaption><p>Execute Service block</p></figcaption></figure>

> ### **Input Pins**

<details>

<summary>AppName</summary>

The Application name that contains the service

Data Type : <mark style="color:orange;">String</mark>

```
Example  :  "Asset"
```

</details>

<details>

<summary>Service</summary>

Name of the model that contains the service, followed by the service call

Data Type : <mark style="color:orange;">String</mark>

```
Example  :  "Asset:All"
```

</details>

<details>

<summary>Parameters</summary>

Required Parameters for executing the service

Data Type : <mark style="color:orange;">Dictionary</mark>

```
Example  :  {}
```

</details>





> ### **Output Pins**

<details>

<summary>AllOutput</summary>

This is the data returned by the service—usually a table service result.

Data Type : <mark style="color:orange;">List</mark>

```
Example  :  [ { "AssetID": 1000, "AssetCategoryKey": 2, "Description": "Operational", "OperationalStatus": null, "OperationalStatusChangeComment": 1, "InstalledLocationKey": null, "Make": null, "Model": null, "SerialNumber": null, "BarCode": null, "InstalledDate": null, "CommissionedDate": null, "Ownership": 0, "IsMobile": null, "ParentAssetKey": null, "PurchasedDate": null, "CurrentAmount": null, "CurrentDepreciationAmount": null, "UpdatedTime": "2024-07-19 05:17:53", "PurchasedAmount": null, "SalvageValue": null, "DisposalDate": null, "WarrantyExpiry": 0, "WarrantyStatus": null, "ClassKey": null, "Specification": null, "OwnerKey": 0, "OwnerType": null, "AssigneeAddedDate": null, "AssigneeKey": null, "AssigneeType": 0, "IsSold": null, "IsBackup": null, "CurrentLocationKey": null, "Manufacturer_VendorKey": null, "Supplier_VendorKey": null, "EndofUsefullLifeDate": 0, "Hidden": 0, "ProfileImageAttachmentKey": 0, "IntegratedAssetKey": null, "WarrantyVendorKey": null, "WarrantyVendorType": null, "WarrantyType": null, "GPSLatitude": 0, "GPSLongitude": 0, "GPSLastUpdatedDateTime": null, "EnableAssetTracking": 0, "CreatedDateTime": "2024-07-01 09:09:20", "CreatedUserKey": 1, "ModifiedDateTime": "2024-07-19 05:17:53", "ModifiedUserKey": 1, "IsLocked": 0, "LockedUserKey": null, "LockedDateTime": null, "AssetKey": 3, "ObjectKey": 3, "__key__": 3, "ObjectID": 1000, "InstalledLocationName": "India", "AssetCategoryID": "Fan", "AssetGroupKey": 0, "AssigneeID": null, "ClassID": "LK", "LoginID": null, "DisplayName": null, "LocationKey": 1, "TimeZone": "HP-Inc", "AssetGroupName": 2, "ParentAssetID": 3, "WarrantyVendorID": null, "__rowid__": null }, { "AssetID": 1001, "AssetCategoryKey": 3, "Description": "Testing asset", "OperationalStatus": "Operational", "OperationalStatusChangeComment": null, "InstalledLocationKey": 1, "Make": "HPAC", "Model": "Version1", "SerialNumber": "QWERTY", "BarCode": "HIHIHIHI", "InstalledDate": "2024-07-04 00:00:00", "CommissionedDate": "2024-07-04 00:00:00", "Ownership": null, "IsMobile": 1, "ParentAssetKey": null, "PurchasedDate": "2024-09-19 06:10:54", "CurrentAmount": null, "CurrentDepreciationAmount": null, "UpdatedTime": "2024-09-19 06:10:54", "PurchasedAmount": null, "SalvageValue": null, "DisposalDate": null, "WarrantyExpiry": 0, "WarrantyStatus": null, "ClassKey": null, "Specification": "Spec", "OwnerKey": 1, "OwnerType": "Organization.OrgBran...", "AssigneeAddedDate": null, "AssigneeKey": null, "AssigneeType": 0, "IsSold": null, "IsBackup": null, "CurrentLocationKey": 0, "Manufacturer_VendorKey": null, "Supplier_VendorKey": null, "EndofUsefullLifeDate": null, "Hidden": null, "ProfileImageAttachmentKey": null, "IntegratedAssetKey": null, "WarrantyVendorKey": null, "WarrantyVendorType": null, "WarrantyType": null, "GPSLatitude": null, "GPSLongitude": null, "GPSLastUpdatedDateTime": null, "EnableAssetTracking": null, "CreatedDateTime": "2024-07-01 07:53:36", "CreatedUserKey": 1, "ModifiedDateTime": "2024-09-19 06:10:54", "ModifiedUserKey": 1, "IsLocked": 0, "LockedUserKey": null, "LockedDateTime": null, "AssetKey": 2, "ObjectKey": 2, "__key__": 2, "ObjectID": "HP-Inc", "InstalledLocationName": "Hong Kong", "AssetCategoryID": "Fan", "AssetGroupKey": 0, "AssigneeID": null, "ClassID": "admin", "LoginID": "Admin", "DisplayName": null, "LocationKey": 2, "TimeZone": "GMT", "AssetGroupName": null, "ParentAssetID": null, "WarrantyVendorID": null, "__rowid__": 2 } ]
```

</details>

<figure><img src="../../.gitbook/assets/General Execute Service Lucy.png" alt=""><figcaption><p>Example: Using the Execute Service block in a real application</p></figcaption></figure>
