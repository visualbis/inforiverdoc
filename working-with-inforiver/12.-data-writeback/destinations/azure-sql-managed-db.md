# Azure SQL (Managed DB)

Allows you to configure a writeback destination in Azure SQL Database that **exists inside & owned by Inforiver tenant**. Recommended for POC purposes only. Users who have difficulties in setting up a database within their tenant are welcome to use this feature to understand Inforiver's writeback functionalities and perform test writebacks for POC purposes.

<figure><img src="../../../.gitbook/assets/image (66) (1).png" alt=""><figcaption><p>Terms of service while using Managed DB</p></figcaption></figure>

After navigating to the writeback destination, enter a name for the writeback table.&#x20;

<figure><img src="../../../.gitbook/assets/image (4) (1).png" alt=""><figcaption><p>Configuration for Inforiver managed Azure SQL</p></figcaption></figure>

After saving the destination, the credentials to access this database will appear on the screen.&#x20;

The user can use this information to access the database using SSMS, Azure Data Studio, or other similar applications. Please note, each table that is configured will have its unique login credentials.&#x20;
