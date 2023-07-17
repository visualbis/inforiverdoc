# Azure Data Lake Storage

Allows you to configure Azure Data Lake Storage as a destination for Inforiver writeback.&#x20;

After navigating to the add destination page, log-in using your O365 credentials.

<figure><img src="../../../.gitbook/assets/image (58).png" alt=""><figcaption></figcaption></figure>

After successful log-in, following details will have to be entered,

* Account
* File System
* Directory
* Partition Required (Y/N)
* Writeback File Name
* Insert Variable

The writeback creates a Parquet file in the data lake storage.&#x20;

**Partition Required:** If the Inforiver scenario is created and included in the writeback, and the user wants to writeback base and scenarios in separate parquet files, this is recommended.&#x20;

**Insert Variables:** Writeback file name can be customized using variables such as Execution ID and date time related IDs.

**Security:** Please note Inforiver leverages Azure Access Control Lists (ACLs) while configuring Azure Data Lake Storage as a writeback destination. That means, the user is only shown folders and directories that they have access to as per the defined ACL rules.

<figure><img src="../../../.gitbook/assets/image (40).png" alt=""><figcaption><p>Configuring Azure Data Lake Storage as a writeback destination</p></figcaption></figure>

##
