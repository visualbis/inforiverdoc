# Azure Data Lake Storage

Allows you to configure Azure Data Lake Storage as a destination for Inforiver writeback.&#x20;

After navigating to the add destination page, log-in using your O365 credentials.

<figure><img src="../../../.gitbook/assets/image (58) (1).png" alt=""><figcaption></figcaption></figure>

After successful log-in, the following details will have to be entered,

* Storage Account
* File System
* Directory
* Partition Required (Y/N)
* Writeback File Name
* Insert Variable

The writeback creates a Parquet file in the data lake storage.&#x20;

<figure><img src="../../../.gitbook/assets/image (10).png" alt=""><figcaption><p>Configure Azure Data Lake Storage destinations</p></figcaption></figure>

**Storage Account:** Enter the name of the Azure Data Lake Storage account

<figure><img src="../../../.gitbook/assets/image (1) (1).png" alt=""><figcaption></figcaption></figure>

**Partition Required:** If the Inforiver scenario is created and included in the writeback, and the user wants to writeback base and scenarios in separate parquet files, this is recommended.&#x20;

**Insert Variables:** Writeback file name can be customized using variables such as Execution ID and date time related IDs.

**Security:** Please note Inforiver leverages Azure Access Control Lists (ACLs) while configuring Azure Data Lake Storage as a writeback destination. That means the user is only shown folders and directories that they have access to as per the defined ACL rules.

### Roles

Ensure that the user has the permissions listed below.

In Inforiver managed mode:

1. Read on the storage account
2. Read and Execute on the file system

<figure><img src="../../../.gitbook/assets/image (2) (1).png" alt=""><figcaption><p>Permissions</p></figcaption></figure>

3. Read, Write, Execute on the folder where the file should be created.

<figure><img src="../../../.gitbook/assets/image (3) (1).png" alt=""><figcaption><p>Folder permissions</p></figcaption></figure>
