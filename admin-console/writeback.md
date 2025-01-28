# Writeback

Inforiver admins can browse all the writeback destinations and filter based on the table name/destination type/created/updated fields from the new Destinations tab. They can also view the configuration details of a particular destination from the Details column.

Admins can use the fields below to apply filters:

* **Table name**: Displays all destinations configured to writeback to the specified table.
* **Destination**: Displays all writeback destinations based on the selected type, E.g. Snowflake, SQL Server, Databricks, Fabric, etc.
* **Create time:** Displays destinations created in the last n minutes/hours/ 7 days/30 days or specified time range.
* **Created/Updated by:** Displays the destinations created or updated by a specific user(s).

<figure><img src="../.gitbook/assets/image (1126) (1).png" alt=""><figcaption><p>Writeback destination management</p></figcaption></figure>

Admins can also view writeback job logs and filter logs. Filters can be applied based on&#x20;

* **Report**: The report name.
* **Started by**:  User(s) that triggered writeback
* **Destination**: Destination type such as BigQuery/ Redshift/Azure data lake&#x20;
* **Environment:**  Service/Desktop/Report Server
* **Status**: Based on the job run status - Success/Failed/Running/Cancelled
* **Event source:** Writeback/ Auto writeback/ Scheduled writeback/ Reset
* **Create time:** Displays job triggered in the last n minutes/hours/ 7 days/30 days or specified time range.

<figure><img src="../.gitbook/assets/image (1127) (1).png" alt=""><figcaption><p>Writeback logs</p></figcaption></figure>

Click the Export button to download the logs to a CSV or Excel file.

<figure><img src="../.gitbook/assets/image (1128) (1).png" alt=""><figcaption><p>Exporting logs</p></figcaption></figure>
