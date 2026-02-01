# Transactions

The **Transactions** tab allows you to link the respective field to a specific DX application and filter the referenced transaction data. This is useful when the field should pull information from another transaction-based app, such as linking to a service request, inspection log, or incident report.

<figure><img src="../../.gitbook/assets/image (129).png" alt=""><figcaption></figcaption></figure>

**Component 1 → DX App**\
The **DX App** dropdown allows you to select the DX app that provides the transaction data for the field.\
This selection is required—without it, the field will not be able to pull or reference any transaction records.

**Component 2 → IQL**  \
The IQL field allows you to define advanced filtering logic using IQL. It lets you narrow down the results shown in the reference field based on specific conditions—like showing only transactions where the status is ‘Open’ or the assigned user matches the current user.

IQL gives you more control and precision when filtering transactions in the form.
