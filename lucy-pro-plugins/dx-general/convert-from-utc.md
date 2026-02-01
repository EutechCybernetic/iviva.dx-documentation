---
description: >-
  The Convert From UTC block allows to convert datetime fields from UTC to a
  specified time zone.
---

# Convert From UTC

<figure><img src="../../.gitbook/assets/Genaral Convert From UTC Lucy.png" alt=""><figcaption><p>Convert From UTC block</p></figcaption></figure>

> ### **Input Pins**

<details>

<summary>Collection</summary>

The Table Service Result List containing multiple table data rows

Data Type : <mark style="color:orange;">List</mark>

```
Example  :  [ { "AssetID": 1000, "AssetCategoryKey": 2, "Description": "Operational", "OperationalStatus": null, "OperationalStatusChangeComment": 1, "InstalledLocationKey": null, "Make": null, "Model": null, "SerialNumber": null, "BarCode": null, "InstalledDate": null, "CommissionedDate": null, "Ownership": 0, "IsMobile": null, "ParentAssetKey": null, "PurchasedDate": null, "CurrentAmount": null, "CurrentDepreciationAmount": null, "UpdatedTime": "2024-07-19 05:17:53", "PurchasedAmount": null, "SalvageValue": null, "DisposalDate": null, "WarrantyExpiry": 0, "WarrantyStatus": null, "ClassKey": null, "Specification": null, "OwnerKey": 0, "OwnerType": null, "AssigneeAddedDate": null, "AssigneeKey": null, "AssigneeType": 0, "IsSold": null, "IsBackup": null, "CurrentLocationKey": null, "Manufacturer_VendorKey": null, "Supplier_VendorKey": null, "EndofUsefullLifeDate": 0, "Hidden": 0, "ProfileImageAttachmentKey": 0, "IntegratedAssetKey": null, "WarrantyVendorKey": null, "WarrantyVendorType": null, "WarrantyType": null, "GPSLatitude": 0, "GPSLongitude": 0, "GPSLastUpdatedDateTime": null, "EnableAssetTracking": 0, "CreatedDateTime": "2024-07-01 09:09:20", "CreatedUserKey": 1, "ModifiedDateTime": "2024-07-19 05:17:53", "ModifiedUserKey": 1, "IsLocked": 0, "LockedUserKey": null, "LockedDateTime": null, "AssetKey": 3, "ObjectKey": 3, "__key__": 3, "ObjectID": 1000, "InstalledLocationName": "India", "AssetCategoryID": "Fan", "AssetGroupKey": 0, "AssigneeID": null, "ClassID": "LK", "LoginID": null, "DisplayName": null, "LocationKey": 1, "TimeZone": "HP-Inc", "AssetGroupName": 2, "ParentAssetID": 3, "WarrantyVendorID": null, "__rowid__": null }, { "AssetID": 1001, "AssetCategoryKey": 3, "Description": "Testing asset", "OperationalStatus": "Operational", "OperationalStatusChangeComment": null, "InstalledLocationKey": 1, "Make": "HPAC", "Model": "Version1", "SerialNumber": "QWERTY", "BarCode": "HIHIHIHI", "InstalledDate": "2024-07-04 00:00:00", "CommissionedDate": "2024-07-04 00:00:00", "Ownership": null, "IsMobile": 1, "ParentAssetKey": null, "PurchasedDate": "2024-09-19 06:10:54", "CurrentAmount": null, "CurrentDepreciationAmount": null, "UpdatedTime": "2024-09-19 06:10:54", "PurchasedAmount": null, "SalvageValue": null, "DisposalDate": null, "WarrantyExpiry": 0, "WarrantyStatus": null, "ClassKey": null, "Specification": "Spec", "OwnerKey": 1, "OwnerType": "Organization.OrgBran...", "AssigneeAddedDate": null, "AssigneeKey": null, "AssigneeType": 0, "IsSold": null, "IsBackup": null, "CurrentLocationKey": 0, "Manufacturer_VendorKey": null, "Supplier_VendorKey": null, "EndofUsefullLifeDate": null, "Hidden": null, "ProfileImageAttachmentKey": null, "IntegratedAssetKey": null, "WarrantyVendorKey": null, "WarrantyVendorType": null, "WarrantyType": null, "GPSLatitude": null, "GPSLongitude": null, "GPSLastUpdatedDateTime": null, "EnableAssetTracking": null, "CreatedDateTime": "2024-07-01 07:53:36", "CreatedUserKey": 1, "ModifiedDateTime": "2024-09-19 06:10:54", "ModifiedUserKey": 1, "IsLocked": 0, "LockedUserKey": null, "LockedDateTime": null, "AssetKey": 2, "ObjectKey": 2, "__key__": 2, "ObjectID": "HP-Inc", "InstalledLocationName": "Hong Kong", "AssetCategoryID": "Fan", "AssetGroupKey": 0, "AssigneeID": null, "ClassID": "admin", "LoginID": "Admin", "DisplayName": null, "LocationKey": 2, "TimeZone": "GMT", "AssetGroupName": null, "ParentAssetID": null, "WarrantyVendorID": null, "__rowid__": 2 } ]
```

</details>

<details>

<summary>Fields</summary>

Fields that need to be converted from UTC to the specified time zone

Data Type : <mark style="color:orange;">String</mark>

```
Example  : "InstalledDate"
```

</details>

<details>

<summary>TimeZone</summary>

The User can specify a time zone, if 'UseUserTimeZone' is set to 0.

Data Type : <mark style="color:orange;">String</mark>

```
Example  : "IST"
```

</details>

<details>

<summary>UseUserTimeZone</summary>

Boolean to indicate whether the field should be converted to the user\`s time zone

Data Type : <mark style="color:orange;">Boolean</mark>

```
Example  : 1
```

</details>

<details>

<summary>UseUserTimeZonISOEnable</summary>

Boolean to indicate whether the datetime field should be formatted as 'yyyy-MM-ddTHH:mm:ssZ'

Data Type : <mark style="color:orange;">Boolean</mark>

```
Example  : 1
```

</details>





> ### **Output Pins**

<details>

<summary>Collection</summary>

Table Service Result List containing multiple table data rows with modified date time fields, such as, InstalledDate

Data Type : <mark style="color:orange;">List</mark>

```
Example  : [ { "AssetID": 1000, "AssetCategoryKey": 2, "Description": "Operational", "OperationalStatus": null, "OperationalStatusChangeComment": 1, "InstalledLocationKey": null, "Make": null, "Model": null, "SerialNumber": null, "BarCode": null, "InstalledDate": null, "CommissionedDate": null, "Ownership": 0, "IsMobile": null, "ParentAssetKey": null, "PurchasedDate": null, "CurrentAmount": null, "CurrentDepreciationAmount": null, "UpdatedTime": "2024-07-19 05:17:53", "PurchasedAmount": null, "SalvageValue": null, "DisposalDate": null, "WarrantyExpiry": 0, "WarrantyStatus": null, "ClassKey": null, "Specification": null, "OwnerKey": 0, "OwnerType": null, "AssigneeAddedDate": null, "AssigneeKey": null, "AssigneeType": 0, "IsSold": null, "IsBackup": null, "CurrentLocationKey": null, "Manufacturer_VendorKey": null, "Supplier_VendorKey": null, "EndofUsefullLifeDate": 0, "Hidden": 0, "ProfileImageAttachmentKey": 0, "IntegratedAssetKey": null, "WarrantyVendorKey": null, "WarrantyVendorType": null, "WarrantyType": null, "GPSLatitude": 0, "GPSLongitude": 0, "GPSLastUpdatedDateTime": null, "EnableAssetTracking": 0, "CreatedDateTime": "2024-07-01 09:09:20", "CreatedUserKey": 1, "ModifiedDateTime": "2024-07-19 05:17:53", "ModifiedUserKey": 1, "IsLocked": 0, "LockedUserKey": null, "LockedDateTime": null, "AssetKey": 3, "ObjectKey": 3, "__key__": 3, "ObjectID": 1000, "InstalledLocationName": "India", "AssetCategoryID": "Fan", "AssetGroupKey": 0, "AssigneeID": null, "ClassID": "LK", "LoginID": null, "DisplayName": null, "LocationKey": 1, "TimeZone": "HP-Inc", "AssetGroupName": 2, "ParentAssetID": 3, "WarrantyVendorID": null, "__rowid__": null }, { "AssetID": 1001, "AssetCategoryKey": 3, "Description": "Testing asset", "OperationalStatus": "Operational", "OperationalStatusChangeComment": null, "InstalledLocationKey": 1, "Make": "HPAC", "Model": "Version1", "SerialNumber": "QWERTY", "BarCode": "HIHIHIHI", "InstalledDate": "2024-07-04T05:30:00Z", "CommissionedDate": "2024-07-04 00:00:00", "Ownership": null, "IsMobile": 1, "ParentAssetKey": null, "PurchasedDate": "2024-09-19 06:10:54", "CurrentAmount": null, "CurrentDepreciationAmount": null, "UpdatedTime": "2024-09-19 06:10:54", "PurchasedAmount": null, "SalvageValue": null, "DisposalDate": null, "WarrantyExpiry": 0, "WarrantyStatus": null, "ClassKey": null, "Specification": "Spec", "OwnerKey": 1, "OwnerType": "Organization.OrgBran...", "AssigneeAddedDate": null, "AssigneeKey": null, "AssigneeType": 0, "IsSold": null, "IsBackup": null, "CurrentLocationKey": 0, "Manufacturer_VendorKey": null, "Supplier_VendorKey": null, "EndofUsefullLifeDate": null, "Hidden": null, "ProfileImageAttachmentKey": null, "IntegratedAssetKey": null, "WarrantyVendorKey": null, "WarrantyVendorType": null, "WarrantyType": null, "GPSLatitude": null, "GPSLongitude": null, "GPSLastUpdatedDateTime": null, "EnableAssetTracking": null, "CreatedDateTime": "2024-07-01 07:53:36", "CreatedUserKey": 1, "ModifiedDateTime": "2024-09-19 06:10:54", "ModifiedUserKey": 1, "IsLocked": 0, "LockedUserKey": null, "LockedDateTime": null, "AssetKey": 2, "ObjectKey": 2, "__key__": 2, "ObjectID": "HP-Inc", "InstalledLocationName": "Hong Kong", "AssetCategoryID": "Fan", "AssetGroupKey": 0, "AssigneeID": null, "ClassID": "admin", "LoginID": "Admin", "DisplayName": null, "LocationKey": 2, "TimeZone": "GMT", "AssetGroupName": null, "ParentAssetID": null, "WarrantyVendorID": null, "__rowid__": 2 } ]
```

</details>

<figure><img src="../../.gitbook/assets/General Convert From UTC.png" alt=""><figcaption><p>Example: Using the Convert From UTC block in a real application</p></figcaption></figure>
