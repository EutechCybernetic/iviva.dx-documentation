---
description: >-
  The Table Field Column Sum block lets you get the sum of values in a table
  column by providing the table structure and the column name.
---

# Table Field Column Sum

<figure><img src="../../.gitbook/assets/Table Field Column Sum.png" alt=""><figcaption><p>Table Field Column Sum block</p></figcaption></figure>



> ### **Input Pins**

<details>

<summary>Simple Table Field</summary>

Defines the structure of the Simple Table&#x20;

Data Type : <mark style="color:orange;">Dictionary</mark>

```
Example  :  { "headings": ["Column1", "Column2", "Column3"], "value": [ [1, 2, 3], [1, 2, 3], [1, 2, 3] ] }
```

</details>

<details>

<summary>Column Name</summary>

The name of the column whose values you want to sum

Data Type : <mark style="color:orange;">String</mark>

```
Example  : Column1
```

</details>





> ### **Output Pins**

<details>

<summary>Column Values</summary>

Sum of the desired column

Data Type : <mark style="color:orange;">Integer</mark>

```
Example  :  3
```

</details>

<figure><img src="../../.gitbook/assets/Table Field Column Sum Lucy.png" alt=""><figcaption><p>Example: Using the Table Field Column Sum block in a real application</p></figcaption></figure>
