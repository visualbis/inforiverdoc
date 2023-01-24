# Inforiver Enterprise

### A) General

#### 1. Is there any installation required for the enterprise edition (SaaS)? <a href="#headline-413-134" id="headline-413-134"></a>

For the SaaS version, there is no installation required. Learn more about the SaaS version [here](https://inforiver.com/enterprise/on-premise-vs-saas/).

#### 2. How can I log in to Inforiver? <a href="#headline-437-2838" id="headline-437-2838"></a>

All Power BI users with a valid Inforiver Enterprise subscription would be able to log in using their Microsoft O365 account.

#### 3. How does the login process work for the admin app/console? <a href="#headline-442-2838" id="headline-442-2838"></a>

You can log in to the admin console by visiting [https://addons.inforiver.com/](https://addons.inforiver.com/). [Admin console](../../advanced-topics/admin-console.md) provides options to manage users, schedules, writeback connections, assets for header/footers, and more. &#x20;

#### 4. How frequently would Inforiver be updated? <a href="#headline-447-2838" id="headline-447-2838"></a>

We are currently on monthly release cycles; we might be shifting to quarterly releases in the future.&#x20;

#### 5. Do I need to be on a Power BI Premium workspace for the enterprise functionality to work? <a href="#headline-452-2838" id="headline-452-2838"></a>

We don't have any requirements on Power BI capacity ​for the enterprise features. One limitation that shared capacity customers might have is if they use the scheduler and want to perform a refresh dataset more than the allowed limit (8 times a day), it wouldn't work.&#x20;

#### 6. What are all the permissions that we need to provide for the Inforiver? <a href="#headline-457-2838" id="headline-457-2838"></a>

Inforiver requires certain permissions to access resources in your organization which must be granted by the O365 admin. Inforiver requires certain permissions to access resources in your organization which must be granted by the O365 admin. &#x20;

<figure><img src="../../.gitbook/assets/FAQ Enterprise permissions.png" alt=""><figcaption><p>Permissions for Inforiver Enterprise</p></figcaption></figure>

#### 7. How to resolve the error showing that the app requires admin consent while login in? <a href="#headline-623-2838" id="headline-623-2838"></a>

Your office 365 administrator has restricted you to use apps that have been consented to by one of the administrators. Follow the steps outlined [here](https://lumel.notion.site/Microsoft-Login-Admin-Consent-b3b8eea861ff4070ab0d586f0b5cc3d7) for your administrator to approve.&#x20;

### B) Writeback

#### 1. Do I have to bring my own database for the writeback? <a href="#headline-795-4237" id="headline-795-4237"></a>

Yes, customers must bring their own destination database for writeback data to be saved for both SaaS as well as on-premise editions. Inforiver will writeback customers' processed data in their configured destination database or other destinations such as OneDrive and SharePoint for data security and data residency compliance purposes. &#x20;

We don't provide any writeback database or any other destinations like SharePoint, OneDrive, etc. for both SaaS and on-premise versions. This is done with the customer's data security considerations in mind as well as it provides maximum flexibility to our architecture where the writeback could be used with cloud data warehouses such as Snowflake, BigQuery, on-premise SQL servers, or SAP HANA.&#x20;

#### 2. What are all the supported destinations for writeback? <a href="#headline-561-2838" id="headline-561-2838"></a>

These are the destinations we support at the moment –&#x20;

Database – Azure SQL, Synapse Analytics Dedicated SQL Pool, Snowflake, Amazon Redshift, BigQuery, SingleStore, SQL server, SAP HANA, Oracle, <mark style="color:red;"></mark> Postgres, and MySQL.

OneDrive and SharePoint – Writeback file as a CSV to the selected folder&#x20;

URL – HTTPS post with the CSV as payload to a configured endpoint&#x20;

#### 3. Does row-level security work with writeback? <a href="#headline-565-2838" id="headline-565-2838"></a>

Yes, you can utilize Power BI Row Level Security (RLS) to restrict data access.&#x20;

#### 4. Can we write back only comments? <a href="#headline-573-2838" id="headline-573-2838"></a>

Yes, cell-level notes and comments are written back. You could use the settings filter option to send only comments.&#x20;

_Note: Comments in categories or column headers are not supported._&#x20;

#### 5. Can we write back only changed values? <a href="#headline-763-4237" id="headline-763-4237"></a>

Yes. You can do this by using the ‘writeback only changes’ option.&#x20;

#### 6. Can we version the writeback data in the destination? <a href="#headline-761-4237" id="headline-761-4237"></a>

Yes. For folder destinations, on creating a new version a new writeback version file will be created. For databases, the writeback version column will be incremented to indicate a new version. Updating the same version which overwrites/replaces the data is also supported.

#### 7. How much volume of data does writeback support? <a href="#headline-755-4237" id="headline-755-4237"></a>

It is optimized for 30,000 rows, but it is subject to vary based on destination and mode of writeback (delta vs filter or collaborative). Writeback to Azure SQL and SQL Server can handle more data volume as we are utilizing a bulk insert approach. Writeback is optimized for up to 100K cells in the July 2022 release and we are looking to improve this further. &#x20;

### C) Commenting

#### 1. Can users add comments in reading mode? <a href="#headline-482-2838" id="headline-482-2838"></a>

Yes, comments can be added in the read mode. The main difference between the edit mode and read mode is the ability to configure additional settings such as restricting access, enabling public commenting, and scheduling summary digests.&#x20;

#### 2. Can users add comments in embedded reports? <a href="#headline-486-2838" id="headline-486-2838"></a>

Inforiver supports ‘Public Commenting’ where users external to the organization can log in in read mode using their Gmail, LinkedIn, or Twitter email ID and add comments.&#x20;

#### 3. What are all the collaboration options available in the comments feature? <a href="#headline-490-2838" id="headline-490-2838"></a>

Inforiver supports collaboration with other users through real-time commenting, email notifications, and commentary digests.   &#x20;

Users can post, reply, and mention users; email notifications are sent on replies and mentions. Authors can restrict access and decide who can post comments in the visual. Comment digests can be scheduled at custom intervals that summarize all comments made between each run.&#x20;

#### 4. When will the users get notified? <a href="#headline-786-4237" id="headline-786-4237"></a>

Users receive email notifications when someone responds to their comments, mentions, or assigns a task to them.&#x20;

#### 5. Is it possible to write back all the comments made in that report? <a href="#headline-502-2838" id="headline-502-2838"></a>

Yes, you can write back notes and comments to databases, shared drives, or URLs. These are the destinations we support at the moment –&#x20;

Database – Azure SQL, Synapse Analytics Dedicated SQL Pool, Snowflake, Amazon Redshift, BigQuery, SingleStore, SQL server, SAP HANA, Oracle, <mark style="color:red;"></mark> Postgres, and MySQL.

OneDrive and SharePoint – Writeback file as a CSV to the selected folder&#x20;

URL – HTTPS post with the CSV as payload to a configured endpoint&#x20;

#### 6. How are notes different from the comments feature? <a href="#headline-506-2838" id="headline-506-2838"></a>

Notes are static texts that do not capture user details. Commenting is a collaboration feature where multiple users can converse over a common thread and the user details and time stamps are recorded. Both notes and comments can be written back to CSV, databases, etc.&#x20;

#### 7. What are all the governance options available for comments? <a href="#headline-510-2838" id="headline-510-2838"></a>

Report authors can limit commentary access to specific users within the domain – this ensures that only those users will be able to view/post comments. Report authors can also delete comments added by other users as necessary or delete all comments.&#x20;

#### 8. Can I get a comment digest periodically? <a href="#headline-736-4237" id="headline-736-4237"></a>

You can configure comments digest for users within the domain – a scheduled summary of the comments at a specified frequency.&#x20;

### D) Scheduler <a href="#headline-522-2838" id="headline-522-2838"></a>

#### 1. Is it possible to schedule reports to an email or other destinations like OneDrive? <a href="#headline-525-2838" id="headline-525-2838"></a>

Custom scheduling of reports to email and other external destinations like OneDrive, SharePoint, and Teams is supported. Burst and broadcast of paginated reports honoring row-level security (RLS) are also possible.&#x20;

#### 2. Is there an ability to burst reports using scheduling? <a href="#headline-529-2838" id="headline-529-2838"></a>

Yes. With Inforiver Enterprise Edition (either as SaaS or On-Premise) – you can set up comprehensive schedules, multiple destinations, and multiple output types (Excel, PDF, Image) for bursting your paginated reports.&#x20;

#### 3. Is it possible to email group mailboxes? <a href="#headline-533-2838" id="headline-533-2838"></a>

Yes, they can specify any email address in the subscription.&#x20;

#### 4. Should the scheduler be set by the report admin, or by the end user? <a href="#headline-537-2838" id="headline-537-2838"></a>

Both the admin and the end user can schedule reports.&#x20;

#### 5. Can we have other Power BI visuals included in the scheduler? <a href="#headline-541-2838" id="headline-541-2838"></a>

No. It is currently limited to Inforiver Matrix, Enterprise, and Charts visuals.&#x20;

#### 6. Can I export all tabs of a Power BI report into excel as a workbook with multiple tabs? <a href="#headline-545-2838" id="headline-545-2838"></a>

Multiple tabs of a Power BI report with Inforiver visuals can be exported as a merged PDF and merged Excel workbook.

#### 7. Can we set up filter rules for the paginated reports? <a href="#headline-549-2838" id="headline-549-2838"></a>

Yes. With the built-in page break feature in Inforiver – the scheduler can handle this feature differently so that the same report could be sent to different individuals based on the page break criteria.&#x20;

#### 8. Is there a way to call/reference the filter on the Email subject or body? <a href="#headline-746-4237" id="headline-746-4237"></a>

Yes, report filters can be included in the email subject/body – refer <mark style="color:red;">post</mark> for more details.&#x20;

#### 9. Can I manually email the paginated reports without requiring Inforiver Enterprise? <a href="#headline-744-4237" id="headline-744-4237"></a>

Yes. With Inforiver Matrix (Premium Edition) – you could manually download the paginated Inforiver PDF export and email your recipients.&#x20;

#### 10. How much volume of data does the scheduler support? <a href="#headline-808-4237" id="headline-808-4237"></a>

Inforiver is optimized for 30,000 rows or about 1,000 pages long. Inforiver is suited for highly visual and formatted paginated reports and is not recommended for large data volume extract type reports.&#x20;

### E) On-Premise <a href="#headline-824-4237" id="headline-824-4237"></a>

#### 1. Is there any installation required for the Enterprise On-Premise edition? <a href="#headline-827-4237" id="headline-827-4237"></a>

Self-hosting within your network in a private azure tenant requires you to deploy our solutions from the Azure Marketplace. Detailed installation and configuration steps for Enterprise On-Premise are available for download[ here](https://inforiver.com/enterprise/on-premise-vs-saas/).\
For further queries, feel free to [reach out to us.](https://inforiver.com/contact-us/)

#### 2. Can Inforiver walk us through the setup and administrative processes of the product? <a href="#headline-831-4237" id="headline-831-4237"></a>

Yes, we will provide a walk-through in our initial discovery call and we will help your deployment team as required.&#x20;

#### 3. What documentation will Inforiver provide on the installation and maintenance? <a href="#headline-835-4237" id="headline-835-4237"></a>

Detailed installation and configuration steps for Enterprise On-Premise are available for download[ here](https://inforiver.com/enterprise/on-premise-vs-saas/). For further queries, feel free [to reach out to us.](https://inforiver.com/contact-us/)

#### 4. What access would Inforiver (company) require to the Inforiver (product) container/VM installed within our Azure? <a href="#headline-839-4237" id="headline-839-4237"></a>

We don't need any access. We can get together with your deployment team and guide them through the entire process.&#x20;

#### 5. What are the communication requirements for the container/VM? <a href="#headline-843-4237" id="headline-843-4237"></a>

All communications would be done on top of https protocol itself.&#x20;

#### 6. Would this Azure container/VM require being exposed outside the internet? <a href="#headline-847-4237" id="headline-847-4237"></a>

Yes, internet connectivity is required for proper functionality. Inforiver on-app premise services require outbound connectivity to Power BI, Azure AD, and Container Registry Service.&#x20;

#### 7. What ports would need to be opened? <a href="#headline-851-4237" id="headline-851-4237"></a>

Only the outbound 443 port needs to be opened. All incoming ports except 443 and other outbound ports can be closed.&#x20;

#### 8. Will any data be transported outside of the direct control of our organization? <a href="#headline-855-4237" id="headline-855-4237"></a>

Your organization would have direct control of the entire data. We don't transport any data to any of our servers. Data can be moved to supporting user-configured services from your org like Writeback database tables, OneDrive, SharePoint, SMTP etc.&#x20;

#### 9. Is there any possibility of running this off AWS, EKS/ECS, or on-prem Kubernetes? <a href="#headline-859-4237" id="headline-859-4237"></a>

Unfortunately, it is not possible right now. But we are looking for other platforms too.&#x20;

#### 10. At what stage of implementation will we perform a sizing evaluation? <a href="#headline-863-4237" id="headline-863-4237"></a>

Before rolling out to the entire company or UAT is completed, we would be able to perform a sizing evaluation and provide proper recommendations.&#x20;

#### 11. What capabilities does Inforiver have around role-based security models? <a href="#headline-869-4237" id="headline-869-4237"></a>

The access is regulated at the granular level and access controls are managed and monitored from Azure PIM.&#x20;

#### 12. How long are the transaction logs available? <a href="#headline-873-4237" id="headline-873-4237"></a>

30 days which is configurable after deployment through Azure Portal.&#x20;

#### 13. How does the transport layer work between the Power BI cloud and Inforiver? <a href="#headline-877-4237" id="headline-877-4237"></a>

We utilize SSL/TLS 1.2 to establish secure communication between Inforiver and Power BI Cloud. The connection establishment and data transfer processes are done as the latest Power BI SDK.&#x20;

#### 14. How is the Inforiver update sent to our Azure subscription (pull/push/automated)? <a href="#headline-881-4237" id="headline-881-4237"></a>

Image Pull update deployment – All the components have an image tag version. When you update and re-deploy, the updates would be pulled directly from our container registry.&#x20;

#### 15. Is there a particular type of server required server to be hosted within our environment? <a href="#headline-885-4237" id="headline-885-4237"></a>

We are using Azure Native cloud services. There is no VM-based deployment.&#x20;

#### 16. How is data sent to this server (authentication, network protocol)? <a href="#headline-889-4237" id="headline-889-4237"></a>

Data is sent through HTTPS protocol and every call would be authenticated by using the JWT auth protocol.&#x20;

#### 17. What are the prerequisites for Inforiver On-Premise? <a href="#headline-893-4237" id="headline-893-4237"></a>

The platform requirements are as below: &#x20;

a. Existing Azure Subscription: A subscription trusts Azure AD to authenticate users, services, and devices. &#x20;

b. New Azure Resource Group: new Azure group will grant the access at resource group level- which makes it simpler to manage and provide greater visibility.&#x20;

c. New Azure AD Application: User will use their domain-based credential to sign in so that users will have a single identity that they can use to access their On-Premise version.

d. SMTP Service Credentials: To enable email notifications in the management console, the user needs SMTP service credentials.&#x20;

SMTP Prerequisites &#x20;

* SMTP Host/Server Address: An SMTP email server will have an address (or addresses) that can be set by the mail client or application that the user is using and is generally formatted as smtp.serveraddress.com&#x20;
* SMTP Username: The user must mention the full email address as SMTP Username, and the email password as the SMTP password in mail configuration settings/coding&#x20;
* SMTP Password: The SMTP password is the same as the web password unless the user is using 2SV. Use smtp.gmail.com, port 465, SSL, or port 587/STARTTLS&#x20;
* SMTP Port: SMTP is used to set up communication rules between the servers &#x20;

e. Inforiver License Key: Prevents illegal use of the software. It is a unique string of characters and numbers provided by Inforiver on the purchase of the product. Users must agree to the terms of the license when acquiring the software.&#x20;

#### 18. What are the resources needed in Azure for deployment? <a href="#headline-897-4237" id="headline-897-4237"></a>

We need the following resources in Azure:&#x20;

1. Azure Web App Service and Plan
2. Azure Kubernetes Service and its dependent Resource Group&#x20;
3. Azure SQL Server and Database
4. Azure Storage Account
5. Azure Cache for Redis
6. Azure Blob Storage
7. Virtual Network and Subnets
8. Private Links and Private Endpoints

#### 19. What would be the Azure cost to maintain the services? <a href="#headline-901-4237" id="headline-901-4237"></a>

Pricing would be based on the estimation [here](https://azure.microsoft.com/en-us/pricing/calculator/?shared-estimate=3e1628c326a84286b7074812b1eb367f). Pricing is subject to change from Azure itself and also based on your component’s usage. &#x20;

#### 20. How does product support work with Inforiver Enterprise (On-Premise)? <a href="#headline-905-4237" id="headline-905-4237"></a>

You can purchase enterprise as a paid add-on, and it is meant for enterprises that require faster turnaround times and assurance. For more details, refer to [https://inforiver.com/support/](https://inforiverstage.wpengine.com/support/). &#x20;
