# Fabric lakehouse

To add a Fabric Lakehouse destination, you need to sign in with Microsoft Office 365 credentials first. After signing in, you will be able to see the list of workspaces and lakehouses that you have access to.&#x20;

<figure><img src="../../../.gitbook/assets/image (372).png" alt=""><figcaption><p>Add Fabric Lakehouse destination</p></figcaption></figure>

1. Select the required workspace and lakehouse.&#x20;
2. Enter the table name.&#x20;
3. When writeback is initiated, the delta csv file is uploaded and the writeback table is created automatically at the specified destination.&#x20;

<figure><img src="../../../.gitbook/assets/1.1. inforiver-simplifies-power-bi-writeback-to-fabric-lakehouse.png" alt=""><figcaption><p>Data writeback completed in lakehouse destination</p></figcaption></figure>

{% hint style="info" %}
The Lakehouse.ReadWrite.All permission needs to be provided to configure lakehouse destinations.
{% endhint %}
