# Get Priorities

The Get Priorities block gives you all the priorities in a DX app. To retrieve them, provide the App Key of the app you are interested in.

<figure><img src="../../.gitbook/assets/Simulate Get Priorities.png" alt=""><figcaption><p>Simulate Get Priorities Block</p></figcaption></figure>

<details>

<summary>AppKey</summary>

This is the App Key for the particular application.

Data Type : <mark style="color:orange;">Integer</mark>

```
Example  :  35
```

</details>

> ### **Output Pins**

<details>

<summary>Priorities</summary>

The priorities of the DX application

Type : List

```
Example  :[ {"id":"PR_1730349986433DLG1DHT8VV","name":"High","color":"#E9573F"}, {"id":"PR_17303499864331IOV1WXXR17","name":"Medium","color":"#e6d700","isDefault":true}, {"id":"PR_1730349986433O3RTLKBKJ2I","name":"Low","color":"#70CA63"} ]
```

</details>

<figure><img src="../../.gitbook/assets/Get Priorities Lucy.png" alt=""><figcaption><p>Example: Using the Simulate Get Priorities Block in a real application</p></figcaption></figure>
