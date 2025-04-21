# Oracle

Allows you to configure Oracle as a destination for Inforiver writeback. You can writeback to a specific instance of an Oracle database using the SID and Service name.

After navigating to the add destination page, enter the following details.&#x20;

* Server
* Service name
* SID
* Port
* Username
* Password
* Encrypted Connection (Y/N)
* Table Name

<figure><img src="../../../.gitbook/assets/image (1) (2) (5) (1).png" alt=""><figcaption><p>Configuring an oracle destination</p></figcaption></figure>

#### Fetching the service name

Enter the service name or SID, which are optional fields. To retrieve the service name from the database, execute the following query

```
SELECT SYS_CONTEXT('userenv', 'service_name') AS service_name FROM dual 
```
