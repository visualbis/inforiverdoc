# Inforiver Matrix FAQs

#### 1.  How do I purchase Inforiver Matrix? <a href="#headline-592-2838" id="headline-592-2838"></a>

Visit Microsoft Appsource to purchase licenses for [Inforiver Matrix](https://appsource.microsoft.com/en-us/product/power-bi-visuals/xviz.inforiver-premium?tab=Overview). Subscription is available by tier and the fee varies based on the plans. To learn how to set up, pay for, and manage licenses for custom Power BI visuals purchased from AppSource, refer to this [article](https://learn.microsoft.com/en-us/power-bi/developer/visuals/licensing-faq).

For other Inforiver licensing-related queries, visit the [General FAQ](https://inforiver.com/faq/) page.

#### 2. Does Inforiver support calculation groups? <a href="#headline-596-2838" id="headline-596-2838"></a>

Yes. Inforiver supports calculation groups as well as all the other native Power BI functionalities. All native Power BI features will work in conjunction with Inforiver features.

#### 3. Your demonstration always shows one visual per page in full-screen mode. Can there also be multiple tables on one page, interacting with each other by filtering? <a href="#headline-661-4516" id="headline-661-4516"></a>

Yes. Inforiver can be used in small form factors just like a native Power BI table/matrix. Inforiver works with slicers and other native visuals and supports multiple cross-filtering.

#### 4. When I export to PDF, why does the font that I have chosen not persist? <a href="#headline-600-2838" id="headline-600-2838"></a>

Inforiver is limited to the 3 MB custom visual size, hence, we are not able to support all the fonts with the Export to PDF feature (each font family is 1MB in size). We were recently able to add "Times New Roman" as an additional font for the Export to PDF feature.

By August 2022 - we switched to the Inforiver font family from Antikor Mono as our default font. As the Inforiver Font family is like Segoe but monospaced for numbers – we think it will be a better default font option. Also, Writeback Matrix customers will be able to use any custom font in the subscription scheduler for the export to PDF feature. This is because the Writeback Matrix has database storage where we could upload additional font styles including custom corporate fonts.

#### 5. Using Display, I can set or change preferences/settings for General, Hierarchy, or Numbers. Can I save my changes permanently or do I have to change settings for each new report? <a href="#headline-604-2838" id="headline-604-2838"></a>

With our enterprise edition – you can save your theme, settings, etc., and it would automatically download them based on your user profile as a corporate theme and default settings. This is possible only with the enterprise edition because we need a DB and server to store and retrieve this configuration.

#### 6. Can I use Inforiver for budgeting/forecasting? <a href="#headline-608-2838" id="headline-608-2838"></a>

Yes. With Inforiver Premium Matrix and Enterprise, you can input and create new budgets or forecasts in seconds. Specifically, you can (a) Create forecasts based on past sales data, (b) Create forecasts from a blank template, (c) Allocate forecasts across countries or product categories proportional to past performance, (d) Perform dynamic what-if simulations to adjust forecasts using a slider interface (e) Comment and annotate on budgets, forecasts, plan, or variance data points, and (f) writeback forecast data along with notes & comments.

Note: Points e and f are supported only in Inforiver Writeback Matrix

Refer to\
1\. Manual Input for Budgets - [Data input, simulations, commenting, and writeback](https://inforiver.com/webinars/data-writeback-in-power-bi-a-deep-dive-and-key-considerations/)\
2\. Advanced Forecasting & What-If Simulations in Microsoft Power BI - [5 ways to run dynamic what-if simulations in Power BI](https://inforiver.com/blog/general/5-ways-to-run-dynamic-what-if-simulations-in-power-bi/)\
3\. Entering Forecasts, Comments, and Write Back - [Forecasting Multiple Items with Seasonality in Power BI](https://inforiver.com/blog/general/forecast-multiple-items-with-seasonality-power-bi/)

However, we suggest using Inforiver to gather your budgets, forecasts, plans, and variance comments using row-level security just like we gather them using Excel spreadsheets.[ ValQ](https://valq.com/) is our recommended advanced planning solution for enterprise use cases. We are working on modernizing ValQ and Integrating with Inforiver where you collect forecast and commentary inputs. ValQ is a separate offering and requires separate purchases for customers needing a full-blown XP\&A or FP\&A or Value Driver Planning solution.

#### 7. Which edition supports export to Excel? <a href="#headline-647-2838" id="headline-647-2838"></a>

All editions support formatted paginated export to Excel in WYSIWYG with structure, format, and notes as is. The Premium edition provides additional customization options for Export to Excel, and they support Export to PDF too. Note: Export to PDF and Excel is possible only in Power BI service. Once you publish your reports, the options should be enabled.

#### 8. What is the performance on large datasets? <a href="#headline-647-2838" id="headline-647-2838"></a>

Inforiver works best with summarized and aggregated data. Your Data model could contain billions of rows, but to leverage the full capabilities of Inforiver, we recommend that you restrict the data assigned to Inforiver using Power BI slicers.

We also offer a performance build where the Inforiver Reporting matrix will function like the native Power BI Matrix by bringing only one hierarchy level at a time for performance reasons but compromising on features/functionalities that require all the hierarchy levels. [Learn more about working with performance mode.](advanced-topics/drill-down-and-roll-up-in-performance-mode.md)

#### 9. Is there a limit to the number of pages that can be exported? <a href="#headline-652-2838" id="headline-652-2838"></a>

We offer a formatted and paginated export solution. There is a limit of 30k rows for Excel and 10MB for PDF for performance and fidelity reasons on the quality of the export.

#### 10. What are the collaboration options available? <a href="#headline-612-2838" id="headline-612-2838"></a>

Inforiver supports [collaboration](https://inforiver.com/collaborate-powerbi/) with other users through real-time commenting, email notifications, scheduled Excel and PDF reports, and commentary digests.

Users can post, reply, and mention users; email notifications are sent on replies and mentions. Authors can restrict access to who can post comments in the visual. Comment digests can be scheduled at custom intervals that summarize all comments made between each run.

However, these options are available only with [Inforiver Enterprise](https://inforiver.com/enterprise/).

#### 11. Can I notify users using comments? <a href="#headline-632-2838" id="headline-632-2838"></a>

Yes, users can be notified using commenting. @ can be used to look up the list of users from one’s organization. This feature is available only in [Inforiver Enterprise.](https://inforiver.com/enterprise/)

#### 12. Can I write back the data from Inforiver to my data source? <a href="#headline-616-2838" id="headline-616-2838"></a>

Inforiver [writeback](https://inforiver.com/writeback-powerbi/) allows users to post the data and comments from the visual to a supported destination. Writeback is supported only in [Inforiver Enterprise](https://inforiver.com/enterprise/) and the following destinations are supported.

Database – Azure SQL, Synapse Analytics Dedicated SQL Pool, Snowflake, Amazon Redshift, BigQuery, SingleStore, SQL server, SAP HANA, Oracle, Postgres, and MySQL.

OneDrive and SharePoint – Writeback file as a CSV to the selected folder&#x20;

URL – HTTPS post with the CSV as payload to a configured endpoint&#x20;

#### 13. Is it possible to schedule reports to email or other destinations like OneDrive? <a href="#headline-642-2838" id="headline-642-2838"></a>

Inforiver [scheduler](https://inforiver.com/schedule-reports-powerbi/) supports custom scheduling of reports to email and other external destinations like OneDrive, SharePoint, and Teams. Burst and broadcast of paginated reports honoring row-level security (RLS) are also possible. This is supported only in [Inforiver Enterprise](https://inforiver.com/enterprise/).&#x20;

#### 14. Can we build our own product incorporating Inforiver and sell it to our customers for a license or subscription free? (OEM licensing) <a href="#headline-656-4516" id="headline-656-4516"></a>

Yes. For bundling (OEM) Inforiver fully or partially with your own products or services to your customers or any third party, a separate licensing plan is available on the [Inforiver website](https://inforiver.com/matrix/pricing/). This would be based on the number of developers or customers.&#x20;

#### 15. Can we build Power BI reports that can be consumed by external organizations for a service fee? (Embedded licensing) <a href="#headline-673-4516" id="headline-673-4516"></a>

Yes. For embedding Inforiver fully or partially with your own products or services, a separate licensing plan is available on the [Inforiver website](https://inforiver.com/matrix/pricing/). This would be based on the number of developers.&#x20;
