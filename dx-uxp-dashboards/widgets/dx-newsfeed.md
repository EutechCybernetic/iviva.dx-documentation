# DX Newsfeed

### 1. Introduction

<figure><img src="../../.gitbook/assets/web and mobile (12).png" alt=""><figcaption></figcaption></figure>

The **DX Newsfeed** widget allows users to stay informed and engaged with updates shared within the DX ecosystem. It displays posts from the newsfeed, encouraging interaction through comments and likes. Whether you are announcing product changes, internal news, or community updates, this widget creates an interactive space for communication.

***

### 2. What Does It Show?

The widget displays individual **newsfeed posts**, including:

* The **title and description** of each update
* The **author and date** of the post
* Interactive options to **like (thumbs up)** or **comment**
* A section that shows **existing comments** below the post
* A field for users to **add new comments**

This setup helps teams and communities engage with each other by acknowledging posts and participating in discussions directly from the dashboard.

***

### 3. Where Does the Data Come From?

This widget pulls content from the built-in **DX Newsfeed** in iviva.DX. It does not require separate configuration for data sources.

{% hint style="info" %}
No data source needs to be configured for this widget.
{% endhint %}

***

### 4. Data Source Component Breakdown (iviva.DX only)

**No data source configuration** is required for this widget. It automatically fetches content from the Newsfeed feature of iviva.DX without needing the user to specify an application or field.

{% hint style="info" %}
**Not applicable** – this widget does not require a data source connection.
{% endhint %}

***

### 5. General Details Component Breakdown

<figure><img src="../../.gitbook/assets/1 - 2025-06-09T020004.896.png" alt=""><figcaption></figcaption></figure>

Below are the configurable options visible in the setup screen:

**Component 1: Title**\
This sets the title shown at the top of the widget (_e.g., Newsfeed_). You can rename it to match your branding or use case (_e.g., Announcements, Team Updates_).

***

### 6. Display Options

The DX Newsfeed widget supports the following display features:

* **Post Display**: Each post includes a title, author, date, content, and category link (_e.g., Rest API_)
* **Like Button (Thumb Icon)**: Users can click to increase the like count. Likes are recorded and shown in real time
* **Comment Box**: Allows users to post comments on a feed items
* **Comment Section**: Displays a list of existing comments under each post, along with the user’s name and timestamp
* **Delete Icon** (for the comment author): Appears next to each comment for users with permission to remove it

These features make the widget suitable for both broadcasting and feedback collection.

***

### 7. Dashboard Visual Breakdown

<figure><img src="../../.gitbook/assets/1 - 2025-06-09T020355.802.png" alt=""><figcaption></figcaption></figure>

Here is how the widget appears on the dashboard, explained by each element:

**Component 1: Widget Title – “NEWSFEED”**\
Displayed at the top, as configured in the General Details section

**Component 2: Post Header**\
Shows the **user’s name** (e.g., Admin User) and **date** (_e.g., 2025-Jun-4_)

**Component 3: Post Title and Subtitle**\
Displays the post title (e.g., _API Development_) and the subtitle (e.g., _Rest API_)

**Component 4: Post Description**\
A paragraph explaining the update or change (e.g., _describing improvements to platform APIs_)

**Component 5: Like and Comment Icons**\
Shows current like and comment counts. Users can click the **thumbs-up icon** to like the post. Users can also see the number of comments displayed next to the comment icon.

**Component 6: Comment Section**\
Displays comments beneath each post. For example:

> **Admin User**\
> &#xNAN;_&#x47;ood info_

**Component 7: Delete Comment Icon**\
Appears next to a comment for the users with permission to delete it

**Component 8: Add Comment Input**\
Allows the user to type a comment and click **COMMENT** to submit it

