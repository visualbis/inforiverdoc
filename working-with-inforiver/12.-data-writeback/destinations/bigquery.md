# BigQuery

Allows you to configure BigQuery as a destination for Inforiver writeback. You can either configure using the JSON or the P12 key type. The details listed in the table below will have to be entered depending on the chosen key type:

| JSON(Recommended) | P12                   |
| ----------------- | --------------------- |
| Dataset ID        | Project ID            |
| Json Key          | Dataset ID            |
| Table Name        | Service Account Email |
|                   | Private Key           |
|                   | Table Name            |

{% hint style="info" %}
* If the tenant administrator creates a connection at admin level, the Dataset ID and Project ID fields will be populated automatically.
* Ensure that the user has permission to SELECT, INSERT, UPDATE, and DELETE data from the table
{% endhint %}

<div><figure><img src="../../../.gitbook/assets/image (1398).png" alt=""><figcaption><p>Configuring BigQuery with JSON key type</p></figcaption></figure> <figure><img src="../../../.gitbook/assets/2025-04-18_17h30_19.png" alt=""><figcaption><p>Configuring BigQuery with P12 key type</p></figcaption></figure></div>

### 1. Generating the JSON key

&#x20;Select the **Create new key** option from the ADD KEY dropdown.

<figure><img src="../../../.gitbook/assets/image (1399).png" alt=""><figcaption><p>Create new key</p></figcaption></figure>

Select the JSON radio button.

<figure><img src="../../../.gitbook/assets/image (1400).png" alt=""><figcaption><p>Choose the JSON option</p></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (1401).png" alt=""><figcaption><p>Key saved notification</p></figcaption></figure>

### 2. Roles

Ensure that the account has “Data Editor” permission.

<figure><img src="../../../.gitbook/assets/image (1402).png" alt=""><figcaption><p>Account should have Data Editor permissions</p></figcaption></figure>
