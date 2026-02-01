---
description: >-
  The Destructure JSON block allows users to destructure a JSON. Users can
  specify which keys to be destructured. The extracted values are then passed
  through the corresponding pins.
---

# Destructure JSON

<figure><img src="../../.gitbook/assets/DX General Destructure JSON.png" alt=""><figcaption><p>Destructure JSON block</p></figcaption></figure>

> ### **Input Pins**

<details>

<summary>JSON</summary>

The JSON value you need to destructure

Data Type : <mark style="color:orange;">Dictionary</mark>

```
Example  :  { "Name": "Alice", "Age": 25, "Location": "New York", "Occupation": "Engineer" }
```

</details>





> ### **Output Pins**

{% hint style="info" %}
#### The Destructure JSON block has multiple output pins.

Users specify which keys in the JSON should be destructured. For example, if the user wants the 'Name',  they can create a output pin called 'Name'.
{% endhint %}

<figure><img src="../../.gitbook/assets/General Destructure JSON Lucy.png" alt=""><figcaption><p>Example: Using the Destructure JSON block in a real application</p></figcaption></figure>
