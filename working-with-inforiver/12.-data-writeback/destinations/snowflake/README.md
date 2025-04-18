# Snowflake

Allows you to configure Snowflake as a destination for Inforiver writeback.&#x20;

After navigating to the add destination page, the following details must be entered, if you choose **Basic Authentication.**

* Account
* Database
* Schema
* Username
* Password
* Warehouse
* Role - ensure the role has 'UASGE' and 'CREATE TABLE' permission
* Encrypted Connection (Y/N)
* Table Name

<figure><img src="../../../../.gitbook/assets/image (1395).png" alt=""><figcaption><p>Configuring snowflake destinations</p></figcaption></figure>

You can also log in using OAuth-type authentication, which ensures a simple and secure login process. The example below illustrates adding a Snowflake destination to an existing integration using OAuth-type authentication. [Learn more about setting up OAuth](setting-up-snowflake-oauth.md).

<figure><img src="../../../../.gitbook/assets/1.3. Snowflake OAuth-updated.png" alt=""><figcaption><p>OAuth-type authentication for Snowflake destination</p></figcaption></figure>

#### - Fetching the role

<figure><img src="../../../../.gitbook/assets/image (1396).png" alt=""><figcaption><p>Fetching the role</p></figcaption></figure>

#### - Fetching the warehouse

<figure><img src="../../../../.gitbook/assets/image (1397).png" alt=""><figcaption><p>Fetching the warehouse</p></figcaption></figure>
