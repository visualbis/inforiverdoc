# Destination Settings

You can add, view, delete, and manage destinations from this tab. Clicking on the manage link will navigate to the destinations page where you can configure and manage your existing destinations.

<figure><img src="../../../.gitbook/assets/image (361).png" alt=""><figcaption><p>Manage destinations</p></figcaption></figure>

### Reset Writeback

If the [writeback filter](general-settings.md#ii-filter) has been changed, a reset is required to clean up the data existing in the destination(s) from previous writebacks. A reset will run a clean-up for both base and scenario data that has been written back to a destination.

For demonstration purposes, consider a SQL server destination to which the base and scenario data have been written back. The count of data populated in the database, region-wise and subregion-wise is as follows:

<figure><img src="../../../.gitbook/assets/image (20) (1) (1) (1) (1).png" alt=""><figcaption><p>Count of region-wise data after writeback</p></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (7) (5) (1).png" alt=""><figcaption><p>Count of subregion-wise data after writeback</p></figcaption></figure>

The filter in writeback settings is changed from "None" to "Exclude Totals and Subtotals":

<figure><img src="../../../.gitbook/assets/image (31) (2) (1).png" alt=""><figcaption><p>Change writeback filter</p></figcaption></figure>

After changing the filter, a reset needs to be done to clean up data from the previous writeback. To achieve this, go to Writeback Settings -> Destinations tab and click on the Reset button.&#x20;

{% hint style="warning" %}
Reset will overwrite data in all configured destinations.&#x20;
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (22) (2) (1).png" alt=""><figcaption><p>Writeback reset</p></figcaption></figure>

Since the filter has been changed to "Exclude Totals and Subtotals", notice that the rows with the value "All" for Region and subRegion have been removed after Reset:

<figure><img src="../../../.gitbook/assets/image (10) (4) (1).png" alt=""><figcaption><p>Count of region-wise data after reset</p></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (28) (3).png" alt=""><figcaption><p>Count of subregion-wise data after reset</p></figcaption></figure>

