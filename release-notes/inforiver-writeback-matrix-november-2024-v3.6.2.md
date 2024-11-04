# Inforiver Writeback Matrix November 2024 - v3.6.2



#### 1. Import data from Google Sheets

Infobridge now ships with built-in compatibility for Google Sheets, unlocking powerful data integration capabilities for users.

<figure><img src="../.gitbook/assets/image (966).png" alt=""><figcaption><p>Sourcing data from Google sheets</p></figcaption></figure>

#### 2. Sourcing data from Lookup visuals

Infobridge provides seamless support for importing single and multi-select data from Lookup visuals. This feature ensures streamlined data transfer from your semantic data models to Infobridge and to child visuals that source data from the bridge.

<figure><img src="../.gitbook/assets/image (967).png" alt=""><figcaption><p>Single and Multi-select support in Infobridge</p></figcaption></figure>

#### 3. Infobridge preview limit

You can preview up to 30k rows before importing data from a bridge into your visual. This allows you to ensure data quality and rectify processing errors prior to integrating data.

<figure><img src="../.gitbook/assets/image.png" alt=""><figcaption><p>Infobridge preview in Inforiver visuals</p></figcaption></figure>



The preview limit is configurable and can be adjusted from the Admin console.

<figure><img src="../.gitbook/assets/image (965).png" alt=""><figcaption><p>Preview limit in the admin console</p></figcaption></figure>

#### 4. Download log files

Analyzing, monitoring, and sharing Inforbrige logs has never been simpler. You can export Infobridge logs from the admin console by navigating to Insights > App Container Logs and selecting the type of logs you need. You have options to export writeback, transformation, and visual logs. This option is primarily intended for on-prem users.

<figure><img src="../.gitbook/assets/image (1).png" alt=""><figcaption><p>Export log files</p></figcaption></figure>



5. **Issue fixes**

* PDF and Excel exports were failing intermittently when visuals had custom row highlights. This issue has been rectified.
* Visual crashes while importing row dimensions with numeric values are now resolved.
