---
description: Unlock Seamless Property & Facility Management with No-Coding.
icon: file-code
---

# DX APIs Documents

The **iviva DX REST API** is a web service that operates over HTTP/HTTPS protocols, enabling third-party applications to communicate seamlessly with **iviva DX** apps. This API provides a set of endpoints that allow external systems to interact with iviva's features and data, supporting seamless integration and process automation. \
By using the iviva DX REST API, developers can access iviva DX services, retrieve data, and perform various actions programmatically, enhancing the functionality and interoperability of their own applications within the  **iviva DX ecosystem**.



<figure><img src="../.gitbook/assets/image (88).png" alt=""><figcaption></figcaption></figure>

**Component 1:** The **API Navigation Panel (sidebar)** allows to easily navigate between different API calls under the DX section. It lists all available endpoints, including options to create, get, submit, and update transactions or checklists.

**Component 2:** The **Endpoint Title** clearly indicates the selected API method—in this case, **Create Transaction**—which is used to create new transactions in a specified app.

**Component 3:** The **Endpoint Description** briefly explains the purpose of the API call, specifying that it enables the creation of transactions for an app.

**Component 4:** The **HTTP Method Badge (POST)** identifies the type of HTTP request used for this API operation.

**Component 5:** The **API Endpoint Path** displays the full endpoint route, including the dynamic segment `{AK}`, which represents the app key.

**Component 6:** The **Path Parameters** section defines variables such as `{AK}` (App Key) that must be included in the endpoint path to execute the call correctly.

**Component 7:** The **Headers** section lists required headers such as **Authorization** (API Key) and **Content-Type**, which must be included in the request for successful execution.

**Component 8:** The **Payload** section outlines the structure of the request body that should be submitted with the POST request. It contains key-value pairs representing the data to be stored in the transaction.

**Component 9:** Clicking this **API Builder Icon** opens a **Build API** popup where you can enter the Base URL and API Key. It also allows you to view and optionally include available payload fields before executing the API call.

**Component 10:** The **Response Body** section displays the structure of the JSON response returned by the API after successful execution.

**Component 11:** The **Error Responses** section provides details about potential error messages or status codes that may occur if the API call fails, assisting with debugging and error handling.
