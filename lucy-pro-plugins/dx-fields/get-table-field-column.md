---
description: >-
  The Get Table Field Column block retrieves the values from a specific column
  in a table by providing the table structure and the column name.
---

# Get Table Field Column



<figure><img src="../../.gitbook/assets/Get Table Field Column.png" alt=""><figcaption><p>Get Table Field Column block</p></figcaption></figure>

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

<summary>Column Name</summary>

The name of the desired column

Data Type : <mark style="color:orange;">String</mark>

```
Example  :  Column1
```

</details>





> ### **Output Pins**

<details>

<summary>Column Values</summary>

Desired Column Values

Data Type : <mark style="color:orange;">List</mark>

```
Example  :  [ "Value1A", "Value1B", "Value1C" ]
```

</details>

<figure><img src="../../.gitbook/assets/Get Table Field Column Lucy.png" alt=""><figcaption><p>Example: Using the Get Table Field Column block in a real application</p></figcaption></figure>
