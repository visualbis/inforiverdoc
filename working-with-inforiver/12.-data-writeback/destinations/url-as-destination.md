# URL as destination

This option allows you writeback into a URL. Inforiver sends the entire writeback table as a JSON to a HTTP endpoint. The endpoint could be a Power Automate workflow that receives the writeback table via the Inforiver JSON where further data processing would take place before storing into a destination such as OneDrive, SharePoint, Dataverse, etc. There are other workflows possible using this method.&#x20;

After navigating to the add destination page enter,

* Endpoint URL
* Required headers and value

<figure><img src="../../../.gitbook/assets/image (64) (1).png" alt=""><figcaption></figcaption></figure>

<pre><code>{"headers":{"Connection":"close",
<strong>"Accept-Encoding":"gzip,deflate",
</strong>"Host":"prod-17.westus.logic.azure.com",
"Content-Length":"583206",
"Content-Type":"application/json"},
"body":{
"data":"\"IrScenario\",\"Productkey\",\"FirstBrand\",\"Category\",\"IrWritebackTimestamp\"\n\
"Base\",\"1\",\"Contoso\",\"Audio\",\"01\",\"2023-04-21 04:05:32 (UTC)\"\n"}}
</code></pre>
