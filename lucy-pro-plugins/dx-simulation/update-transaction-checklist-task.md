# Update Transaction Checklist Task

The Simulate Update Transaction Checklist Task block lets you update the details of a task in a transaction's checklist. To update the task, you need to provide the App Key, Transaction Key, Map Key, and Task Index.

<figure><img src="../../.gitbook/assets/Update Transaction Checklist Task.png" alt=""><figcaption><p> Simulate Update Transaction Checklist Task block </p></figcaption></figure>

> ### **Input Pins**

{% hint style="info" %}
#### The Simulate Update Transaction Checklist Task block has multiple input pins.

You can update the following pins: `TaskValue`(user defined type), `Comments`(string list),and `IsCompleted`(boolean).


{% endhint %}

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

This is the Transaction Key of the required transaction.

Data Type : <mark style="color:orange;">Integer</mark>

```
Example  :  1
```

</details>

<details>

<summary>MapKey</summary>

The Checklist Map Key of the required checklist in the transaction

Data Type : <mark style="color:orange;">Integer</mark>

```
Example  :  1
```

</details>





> ### **Output Pins**

<details>

<summary>AppKey</summary>

This is the app key for a particular application

Data Type : <mark style="color:orange;">Integer</mark>

```
Example  :  36
```

</details>

<details>

<summary>TransactionKey</summary>

This is the Transaction Key of the required transaction.

Data Type : <mark style="color:orange;">Integer</mark>

```
Example  :  1
```

</details>

<details>

<summary>MapKey</summary>

The Checklist Map Key of the required checklist in the transaction

Data Type : <mark style="color:orange;">Integer</mark>

```
Example  :  1
```

</details>

<details>

<summary>TaskIndex</summary>

Index of the task in the task list in the transaction checklist

Data Type : <mark style="color:orange;">Integer</mark>

```
Example  :  1
```

</details>

<figure><img src="../../.gitbook/assets/Simulate Update Transaction Checklist Task.png" alt=""><figcaption><p>Example of using the Simulate Update Transaction Checklist Task in a real application</p></figcaption></figure>
