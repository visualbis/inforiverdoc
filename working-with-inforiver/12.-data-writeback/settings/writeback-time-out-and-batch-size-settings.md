# Writeback time-out & batch size settings

Admins can adjust the request timeout duration and the batch size for writebacks in the admin console, especially when working with high-volume data, to achieve superior performance.

## 1. Request Time out

When Inforiver cannot connect to a writeback destination within the specified time limit, it displays a request timeout error. You can now set a custom connection time from the admin console which gives ample time for Inforiver to connect to a destination before displaying a time-out error.

In the admin console, navigate to **Settings** and then Writeback > Settings. Under the **Writeback destination connection** settings, you can set the duration of the request time-out. In the example, we have set it to 300 seconds. Inforiver will wait up to 300 seconds for the connection to be established before generating a request timeout error.&#x20;

<figure><img src="../../../.gitbook/assets/image (926).png" alt=""><figcaption><p>Request timeout</p></figcaption></figure>

## 2. Batched Write Setting

By default, if your writeback payload exceeds 50k records, Inforiver can split the payload into multiple chunks and write them back batch-by-batch. To know how to configure batched writeback and specify the temporary table for holding the batched data, you can refer to [this section](../destinations/#id-3.-batch-writeback).

You can change the default batch size of 50k records in the **Batched Write Setting** section. In the example below, we have specified the batch size as 75k. Batched writeback happens when the writeback payload exceeds 75k records with each chunk size of 75k records.

<figure><img src="../../../.gitbook/assets/image (927).png" alt=""><figcaption><p>Batch size</p></figcaption></figure>
