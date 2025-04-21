# Fabric Warehouse

After navigating to the add destination page, the following details are required to add **Fabric Warehouse** as a writeback destination:

* SQL connection string
* Database name
* Schema name
* Client ID
* Client secret
* Table name

<figure><img src="../../../.gitbook/assets/image (293).png" alt=""><figcaption><p>Fabric warehouse</p></figcaption></figure>

#### Fetching the DB name and connection string

<figure><img src="../../../.gitbook/assets/image (1403).png" alt=""><figcaption><p>DB name and connection string</p></figcaption></figure>

#### Fetching the Service Principal Client ID and Service Principal Client Secret

Refer to the highlighted fields in the screenshot below to get the Service Principal Client ID. Client Secret is obtained while creating the Service Principal Account.

<figure><img src="../../../.gitbook/assets/image (1404).png" alt=""><figcaption><p>Fetching the service principal client ID</p></figcaption></figure>

#### Additional configuration for optimised insert

To perform bulk insert when there is large data, ensure these items are configured:

1\. Create a **"Workspace Identity"** and then add the **"Service Principal"** as an **"Authorized User"**.

<figure><img src="../../../.gitbook/assets/image (1405).png" alt=""><figcaption></figcaption></figure>

2\. Ensure that the **"Workspace Identity"** is whitelisted in the **"Resource Instance Rules"** of th&#x65;**"Storage Account"**.

<figure><img src="../../../.gitbook/assets/image (1406).png" alt=""><figcaption></figcaption></figure>
