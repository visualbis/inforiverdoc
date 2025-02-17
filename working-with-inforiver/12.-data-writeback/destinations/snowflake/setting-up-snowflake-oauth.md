# Setting up Snowflake OAuth

This section outlines the steps required to create an integration and use OAuth to connect to Snowflake.

### 1. Prerequisites

* Whitelist Inforiver IPs in the Azure SQL firewall. [Learn more about whitelisting Inforiver IPs](../../../../introduction-to-inforiver/get-started/inforiver-writeback-matrix-pre-requisites/whitelist-inforiver-ips.md).
* For Saas customers, [https://addons.inforiver.com](https://addons.inforiver.com) should be whitelisted in the firewall so the application can reach the server configured.

### 2. Creating an integration in Snowflake

**STEP 1:** Use the ACCOUNTADMIN role to log in to the Snowflake web interface. Navigate to Projects -> Worksheets -> Click the Add icon at the top left -> Select SQL worksheet.

**STEP 2:** Create an OAuth Security Integration by executing the query:

<pre class="language-sql"><code class="lang-sql">CREATE SECURITY INTEGRATION MY_INTEGRATION_NAME
TYPE = OAUTH
ENABLED = TRUE
OAUTH_CLIENT = CUSTOM
OAUTH_CLIENT_TYPE = 'CONFIDENTIAL'
<strong>OAUTH_REDIRECT_URI = '&#x3C;Redirect link>'
</strong>OAUTH_ISSUE_REFRESH_TOKENS = TRUE
OAUTH_REFRESH_TOKEN_VALIDITY = 86400; -- set OAUTH Refresh token validity from 1 to 90 days (about 3 months) in seconds 
</code></pre>

**STEP 3:** Fetch details for client configuration. You will need to enter these details while creating a Snowflake destination or connection in Inforiver.

Retrieve the Client ID and Client secret:

```sql
SELECT SYSTEM$SHOW_OAUTH_CLIENT_SECRETS( 'MY_INTEGRATION_NAME');
//OAUTH_CLIENT_ID => Client ID field in Inforiver console
//OAUTH_CLIENT_SECRET => Client Secret field in Inforiver console
```

Get the Authorization and Token URL:

```sql
DESC SECURITY INTEGRATION MY_INTEGRATION_NAME;
//OAUTH_AUTHORIZATION_ENDPOINT => Authorization URL field in Inforiver console
//OAUTH_TOKEN_ENDPOINT => Token URL field in Inforiver console
```

### 3. Using OAuth to create a destination or connection in Inforiver

**STEP 1:** Enter the **Integration Name**, **Client ID**, **Client Secret**, **Authorization URL**, and **Token URL** required for OAuth in the Inforiver console. Refer to the [previous section ](setting-up-snowflake-oauth.md#id-1.-creating-an-integration-in-snowflake)to learn more about fetching the integration details from Snowflake. Click **Connect**.

<figure><img src="../../../../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Enter integration details for Snowflake</p></figcaption></figure>

You will be redirected to the Snowflake login page, where you need to enter your Username and Password to connect.

<figure><img src="../../../../.gitbook/assets/image (3) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt="" width="375"><figcaption><p>Snowflake Sign in</p></figcaption></figure>

### 4. Enter Account/DB/Schema/Warehouse details

After specifying the integration details for OAuth and signing into Snowflake, you will need to enter details in the section highlighted in the image:

<figure><img src="../../../../.gitbook/assets/image (7) (1) (1) (1) (1) (1) (1) (1) (1).png" alt="" width="563"><figcaption></figcaption></figure>

* **Account**: Enter the name of your Snowflake server. Example: https://\<account>.snowflakecomputing.com/
* **Database and Schema:** Snowflake Database and schema name where the writeback table will be created.

<figure><img src="../../../../.gitbook/assets/image (4) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Snowflake database and schema</p></figcaption></figure>

* **Warehouse:** The Snowflake compute warehouse.

<figure><img src="../../../../.gitbook/assets/image (5) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Snowflake warehouses</p></figcaption></figure>

* **Role**: The user role associated with the Snowflake username.  Ensure this role has “USAGE” and “CREATE TABLE” permissions. This is mandatory to be able to writeback from Inforiver to Snowflake.

<figure><img src="../../../../.gitbook/assets/image (6) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Snowflake roles</p></figcaption></figure>
