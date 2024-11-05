# Inforiver Writeback Matrix November 2024 - v3.6.2

Experience data integration in Power BI on an entirely new scale with Infobridge support for Google Sheets and Lookup Visuals. This release focuses on improving stability with options to download container logs and export/import queries. Let's explore the highlights:

#### 1. Import data from Google Sheets

Infobridge now ships with built-in compatibility for Google Sheets, unlocking powerful data integration capabilities for users.

<figure><img src="../.gitbook/assets/image (966).png" alt=""><figcaption><p>Sourcing data from Google Sheets</p></figcaption></figure>

#### 2. Sourcing data from Lookup visuals

Infobridge provides seamless support for importing single and multi-select data from Lookup visuals. This feature ensures streamlined data transfer from your semantic data models to Infobridge and child visuals that source data from the bridge.

<figure><img src="../.gitbook/assets/image (967).png" alt=""><figcaption><p>Single and Multi-select support in Infobridge</p></figcaption></figure>

#### 3. Infobridge preview limit

You can preview up to 30k rows within Infobridge. This allows you to ensure data quality and rectify processing errors before integrating data with other visuals.

<figure><img src="../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

The preview limit is configurable and can be adjusted from the Admin console.

<figure><img src="../.gitbook/assets/image (965).png" alt=""><figcaption><p>Preview limit in the admin console</p></figcaption></figure>

#### 4. Download log files

Analyzing, monitoring, and sharing Inforbrige logs has never been simpler. You can export Infobridge logs from the admin console by navigating to Insights > App Container Logs and selecting the type of logs you need. You have options to export writeback, transformation, and visual logs. This option is primarily intended for on-prem users.

<figure><img src="../.gitbook/assets/image (1) (1).png" alt=""><figcaption><p>Export log files</p></figcaption></figure>

#### 5. **Export and import from Infobridge**

After applying various transformations to your data, you may need to export the transformed data and integrate it with an additional bridge for further processing or connectivity. You will now be able to export your queries and import them.

#### **6. Issue fixes**

* PDF and Excel exports were failing intermittently when visuals had custom row highlights. This issue has been rectified.
* Visual crashes while importing row dimensions with numeric values are now resolved.

**Learn more about Inforiver** &#x20;

To learn more about the latest from [Inforiver](https://inforiver.com/why-inforiver/) and why we are garnering recognition from industry experts, check out our newest [brochure](https://inforiver.com/wp-content/uploads/inforiver-brochure.pdf). &#x20;

Inforiver and all our planning and analytics products continue to be updated to provide a diverse range of users with optimal performance. With continual improvements and innovations planned, we welcome your feedback.       &#x20;

If you’re ready to level up your planning, reporting, and analytics, [try our products](https://inforiver.com/products/) for free today.  
