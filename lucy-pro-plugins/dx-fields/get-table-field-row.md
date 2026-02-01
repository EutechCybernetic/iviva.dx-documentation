---
description: >-
  The Get Table Field Row block allows you to get the values from a specific row
  in a table by providing the table structure and the row number.
---

# Get Table Field Row



<figure><img src="../../.gitbook/assets/Get Table Field Row.png" alt=""><figcaption><p>Get Table Field Row block</p></figcaption></figure>

> ### **Input Pins**

<details>

<summary>Simple Table Field</summary>

Defines the structure of the Simple Table&#x20;

Data Type : <mark style="color:orange;">Dictionary</mark>

```
Example  :  { "headings": ["Column1", "Column2", "Column3"], "value": [ ["Value1A", "Value2A", "Value3A"], ["Value1B", "Value2B", "Value3B"], ["Value1C", "Value2C", "Value3C"] ] }
```

</details>

<details>

<summary>Row Number</summary>

The row number of the particular table row



Data Type : <mark style="color:orange;">String</mark>

```
Example  : 1
```

</details>





> ### **Output Pins**

<details>

<summary>Row</summary>

Desired Row Values

Data Type : <mark style="color:orange;">List</mark>

```
Example  : [ "Value1A", "Value2A", "Value3A" ]
```

</details>

<figure><img src="../../.gitbook/assets/Get Table Field Row Lucy.png" alt=""><figcaption><p>Example: Using the Get Table Field Row block in a real application</p></figcaption></figure>
