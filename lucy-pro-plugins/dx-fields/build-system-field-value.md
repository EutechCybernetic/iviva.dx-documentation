---
description: >-
  The Build System Field Value block lets you return the field value from an
  iviva object type.
---

# Build System Field Value

<figure><img src="../../.gitbook/assets/Simulate Build System Field Value.png" alt=""><figcaption><p>Build System Field Value block</p></figcaption></figure>



<details>

<summary>FieldValue</summary>

This is a unique key for choosing the particular iviva object type value.

Data Type : <mark style="color:orange;">Integer</mark>

```
Example  :  1
```

</details>

<details>

<summary>IvivaObjectType</summary>

This is the type of the iviva object.

Data Type : <mark style="color:orange;">String</mark>

```
Example  :  Asset | Location | User
```

</details>

<details>

<summary>AppInstanceKey</summary>

This is the instance key for a specific working instance of the application.

Data Type : Integer

```
Example  :  23
```

</details>



> ### **Output Pins**

<details>

<summary>Value</summary>

The result of the generated system field value

Data Type : **Dictionary**

```
Example  :  {"Value":"1","DisplayText":"Administrator"}
```

</details>

<figure><img src="../../.gitbook/assets/simulate Build System Field Value Lucy.png" alt=""><figcaption><p>Example: Using the Build System Field Value block in a real application</p></figcaption></figure>
