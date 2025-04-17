# Inforiver Writeback Matrix November 2024 - v3.6.2 - Import from Google Sheets & More

Data integration in Power BI just got easier with the new Infobridge support for Google Sheets and Lookup Visuals. This latest release offers enhanced stability with options to download container logs and export/import queries.&#x20;

Discover the new features in version 3.6.2:

#### 1. Import data from Google Sheets

Infobridge now ships with built-in compatibility for Google Sheets, bringing powerful data integration capabilities to users. Navigate to Home > Add Source and select the file(s) from your Google Drive account.

{% hint style="info" %}
In order to fetch data from Google Sheets, connect to the associated Google Drive account from the Admin Console > Profile > My Integrations section.
{% endhint %}

<figure><img src="../.gitbook/assets/image (966).png" alt=""><figcaption><p>Sourcing data from Google Sheets</p></figcaption></figure>

#### 2. Single and multi-select data from Lookup visuals

Infobridge now provides support for importing single and multi-select data from Lookup visuals. This feature ensures streamlined data transfer from your semantic data models to Infobridge and child visuals that source data from the bridge.

<figure><img src="../.gitbook/assets/image (967).png" alt=""><figcaption><p>Single and Multi-select data from Lookup visual published to Infobridge</p></figcaption></figure>

#### 3. Infobridge preview limit

You can preview up to 30k rows within Infobridge. This allows you to load a larger volume of data before integrating it with other visuals.

<figure><img src="../.gitbook/assets/image (11) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

The preview limit is configurable and can be adjusted from the Admin console.

<figure><img src="../.gitbook/assets/image (965).png" alt=""><figcaption><p>Preview limit in the admin console</p></figcaption></figure>

#### 4. Download log files

Analyzing, monitoring, and sharing Infobridge logs has never been simpler. You can export Infobridge logs from the admin console by navigating to Insights > App Container Logs and selecting the type of logs you need. You have options to export writeback, transformation, and visual logs. This option is primarily intended for on-prem users and is not available for SaaS customers.

<figure><img src="../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1)  (10).png" alt=""><figcaption><p>Export log files</p></figcaption></figure>

#### 5. **Export and import from Infobridge**

After applying various transformations to your data, you may need to export the transformed data and integrate it with an additional bridge for further processing.&#x20;

The Export option will be enabled when you transform data within Infobridge. Navigate to the Transform ribbon and click Export to download your query as a .bck file.&#x20;

<figure><img src="../.gitbook/assets/image (968).png" alt=""><figcaption><p>Import and Export in Infobridge</p></figcaption></figure>

#### **6. Issue fixes**

* PDF and Excel exports were failing intermittently when visuals had custom row highlights. This issue has been rectified.
* Visual crashes while importing row dimensions with numeric values are now resolved.
* Copy-paste issues in the MoR layout have been resolved.

**Learn more about Inforiver** &#x20;

To learn more about the latest from [Inforiver](https://inforiver.com/why-inforiver/) and why we are garnering recognition from industry experts, check out our newest [brochure](https://inforiver.com/wp-content/uploads/inforiver-brochure.pdf). &#x20;

Inforiver and all our planning and analytics products continue to be updated to provide a diverse range of users with optimal performance. With continual improvements and innovations planned, we welcome your feedback.       &#x20;

If you’re ready to level up your planning, reporting, and analytics, [try our products](https://inforiver.com/products/) for free today.  
