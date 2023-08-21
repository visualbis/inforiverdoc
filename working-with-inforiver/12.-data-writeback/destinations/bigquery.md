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
If the tenant administrator creates a connection at admin level, the Dataset ID and Project ID fields will be populated automatically.
{% endhint %}

&#x20;For more information regarding setting up BigQuery destinations, refer to the help section at the top left of the page:

<figure><img src="../../../.gitbook/assets/image (12).png" alt=""><figcaption><p>BigQuery writeback</p></figcaption></figure>

