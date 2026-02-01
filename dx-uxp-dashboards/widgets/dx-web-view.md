# DX Web View

**1. Introduction**

<figure><img src="../../.gitbook/assets/web and mobile9.png" alt=""><figcaption></figcaption></figure>

The **DX Web View** widget lets you embed a web page or internal application view right into your dashboard. The widget supports setting up dynamic URLs with parameters, so that different users or contexts get routed to the right records or pages.

***

**2. What Does It Show?**

The DX Web View widget shows a web page (e.g., a DX application record view) right inside the widget space. It can display any external or internal link—like a location profile, user page, or asset detail—based on the parameters passed in the URL.

***

**3. Where Does the Data Come From?**

{% hint style="info" %}
You do not need to configure a data source for the DX Web View widget. Just enter location coordinates and choose your visual settings to set up a visual map.
{% endhint %}

***

**4. Data Source Component Breakdown**

{% hint style="info" %}
There’s **no data source panel to configure** when you choose the iviva.DX option. The widget automatically pulls in related assets based on the current context—no extra setup needed.
{% endhint %}

***

**5. General Details Component Breakdown**

<figure><img src="../../.gitbook/assets/1 - 2025-06-09T170956.493.png" alt=""><figcaption></figcaption></figure>

**Component 1: Title**\
Set the title that appears at the top of the widget. It should describe what the embedded page is about—like _Location Overview_

**Component 2: Web View Link**\
Enter the URL of the web page you want to embed. You can add parameters in the format `#{parameterName}` to make the link update dynamically based on the setup below.

**Component 3: Parameters**\
This section allows you to define and manage dynamic values that can be inserted into your URL.

For example, if your URL includes `key=#{UserKey}`, you can define a parameter called **UserKey** and choose one of these parameter types:

* **Static**: Manually assign a fixed value
* **Environment**: Pick one of the values listed from the system environment
* **List**: Select a value dynamically (e.g., current user or other predefined options)

> These three types (`Static`, `Environment`, and `List`) follow the format: `key=#{UserKey}`.

If the parameter type is **Query String**, format your URL like this:

```
key=#{QS.UserKey}
```

In this case, define a parameter called **UserKey**  and set its type to **Query String**.

Click here to explore more about how [Parameter Configuration ](./#parameter-configuration)works.

***

**6. Display Options**

The DX Web View widget does not offer advanced styling options. The embedded web view appears as it is, based on the widget’s size and height on the dashboard. Any formatting comes from the linked page itself—not from the widget.

***

**7. Dashboard Visual Breakdown**

<figure><img src="../../.gitbook/assets/1 - 2025-06-09T171202.702.png" alt=""><figcaption></figcaption></figure>

**Component 1: Title Bar**\
Shows the title configured in the 'Title' field (_e.g., WebView_)

**Component 2: Embedded Page**\
Displays the target page specified in the link. In this example, it loads a specific location profile from the iviva.DX system, including details like Location Name, Type, and layout-specific tabs.
