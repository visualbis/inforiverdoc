# Power BI Writeback is as easy as 1-2-3

by Inforiver | Aug 05, 2022 | [Inforiver Enterprise](https://inforiver.com/blog/category/inforiver-enterprise/), [Writeback](https://inforiver.com/blog/category/writeback/)\


Performing a database writeback from Power BI can get highly technical and effort-intensive, requiring advance setup, configuration and coding. However, with Inforiver for Power BI, you can perform your first writeback in a matter of minutes without writing a single line of code.

In this tutorial, we will explore how you can use Inforiver visual in Power BI to perform the following in a matter of minutes:

1. **Write back values, text & comment data** from your Power BI matrix to a database or shared drive (we will use Snowflake in our example).
2. **Perform a writeback without creating a database table in advance –** we call this ‘unstructured writeback’ or ‘free-form writeback’ (a market-leading capability offered by Inforiver, which provides you with the speed & agility unseen in any other writeback product). This **IS** the _**fastest way to perform a writeback**_ in Power BI.
3. Leverage several options for writeback (_without writing any code_) such as
   * Set up writeback permissions to specific users (within your Power BI report)
   * Write back only data that have comments
   * Write back a filtered data set (vs. writing all records)
   * Perform incremental or full writeback
   * Overwrite existing writeback data or create new records every time
   * Include totals or totals/subtotals while writing back a table or matrix
   * … and more.

You can accomplish this writeback in 3 easy steps using Inforiver.

1. **Configure writeback destination**
2. **Configure writeback options**
3. **Write back data**

Let us go through this with an example.

We have data for 2022 Sales Actuals in this Power BI report built using Inforiver Enterprise.

We have now gone ahead and entered forecast for the year 2023 by Quarter, and also added status & comment columns to track the progress of this effort. Learn how you can [manually input data in your Power BI report](https://inforiver.com/blog/writeback/5-types-manual-data-entry-powerbi-table-matrix/) using Inforiver.

All of this additional data now resides in the visual. It needs to be written back to a database. Let us do this in three (3) easy steps.

### STEP 1: CONFIGURE WRITEBACK DESTINATION

The first step in choosing a writeback destination is allow Inforiver to authenticate you. You’ll notice the ‘Sign in’ button on the top right. When you click on this button, or when you try to select ‘Writeback’ without signing in, you will be prompted to sign in with Office 365.

Click on the button. If you are already signed into Office 365 in your system, you need not enter your credentials again. Inforiver will authenticate you automatically, after which you will see your name on the top right.

Now that you have signed in, click on the ‘Writeback’ icon in the toolbar.

Note that we are performing writeback for the first time from this report. Since no destination has been configured for this report, Inforiver will open a portal automatically and prompt you to choose a specific destination.

For our exercise, we will ignore the destinations listed and instead set up a new destination from scratch. Click on the ‘Database’ option. This will reveal several options. Note that you can write back from Power BI to Azure SQL, SQL Server, Snowflake, BigQuery, SAP HANA, PostgreSQL and MySQL using Inforiver. We will choose Snowflake and click 'Continue'.

A side note - similar to the 'Database' list, choosing ‘Files’ on the popup window shown above will reveal two options – OneDrive & SharePoint.

You can also write back to a URL, and this option is available in the ‘Others’ pane.

We will stick to our choice of Snowflake database and will click the ‘Continue’ button in the popup window. This will prompt us to provide additional details for the destination – such as the schema name, username, password etc.,

Note that we are giving the table name as **WRITEBACK\_STEPBYSTEP**. However this table does not exist in Snowflake yet.

Click on ‘Save Destination’ button in this page on the top right. You will get a confirmation screen.

The destination setup is now complete.

**Note:** As mentioned earlier, the table WRITEBACK\_STEPBYSTEP does not exist in Snowflake yet. We are only telling Inforiver to write to a table named WRITEBACK\_STEPBYSTEP. When Inforiver does not find a table with this name, it will trigger a CREATE TABLE query automatically during runtime. This gives you a lot of flexibility on what to write back, which measures to include etc., until the very moment you perform the writeback action. We will explore this further in a few steps.

If you try to locate this table WRITEBACK\_STEPBYSTEP in Snowflake now, you will not see it. When we search for tables containing the term WRITEBACK in their name, you will only see other tables meeting this criteria.

### STEP 2: CONFIGURE WRITEBACK OPTIONS

Now that we have defined WHERE to write back, let us take a few seconds to determine WHAT to write back. In our Power BI report, click on ‘Settings’ in the tool bar. This will open the Writeback Settings tab.

The settings chosen in the image indicate that we want to

* write back only the 2023 projections along with status & comments (and ignore 2022 Actuals)
* write back all the records every time we perform a writeback (not a delta writeback), and
* exclude writing back totals & subtotals in the matrix

You will observe more options under the Filter Section. You can note that Inforiver allows you to write back

* only data with corresponding comments,
* only calculated rows or
* write back a filtered data set.

We are not exercising these options for now.

Choosing the option ‘Custom Filters’ will let us enter the filter criteria on the data. Only the records matching the filter criteria will be written back. For example, we can write back data pertaining to only home appliances category. However, for this walkthrough, we will stick to the filter option ‘Exclude Totals and Subtotals’.

In the Writeback Settings pane, when you switch to the ‘Destination’ tab, you will see the destination(s) available to this report. This is the same destination that we created in Step #1. You can create multiple destinations for a single report.

The last tab ‘Others’ allows you to set user permissions. If you want only specific users in your domain to write back data from this report, you can set it up here.

Once you have set up the writeback configuration, go ahead and click on Save.

After having set up the destination and configuring writeback properties in the first two steps, we are now ready to write back data to Snowflake. Note that all of the items that we configured in step #2 can be set up only by report designers (with edit rights). However, the actual writeback can be performed by users in reading mode too. Since you may not want all users to perform a writeback, the ability to restrict permissions to specific users can be highly helpful.

### STEP 3: WRITE BACK DATA

Finally, we are ready to write back data. Click on the Writeback button from the toolbar now.

Now that we are already authenticated, and we have a destination defined, Inforiver reconfirms WHAT you are writing back (refer image below). As mentioned earlier in Step #2, if you do not have a destination defined, it will take you to the web portal to set up a destination for this report.

In the popup below, you will notice that the options that you selected in step #2 are highlighted. You can change them now if you need.

You will also notice another new property in the image above named ‘Writeback Version’. While writing back, Inforiver gives you two options – overwrite existing version of the data in the database or create a new version. Choosing the 'Create New Version' option ensures that all the past writeback records from this report remain untouched.

Navigating to the other two tabs in the popup – _Destinations_ & _Settings_ – allows you to review all other properties we had configured in Steps #1 and #2.

In the Destinations tab, you can choose to write back to multiple destinations simultaneously using the check box (provided multiple destinations are set up for this report). Clicking on ‘Manage Destinations’ from this popup will take us to the same portal that we explored in Step #1.

The Settings tab summarizes other options that we had set up earlier.

Once you are satisfied with the configuration, click on Writeback. You will see the live status of writeback appear on the top right.

You will soon receive a prompt saying that the writeback is complete.

Clicking on ‘View Log’ in the screen above opens the portal where you can view a more detailed status. This is useful for administration & troubleshooting.

Finally, when you query Snowflake database now, you will see a new table **WRITEBACK\_STEPBYSTEP** inserted by Inforiver at runtime. Note that we did not create this table ahead of time. Inforiver created this on-the-fly based on the columns we chose for writeback.

As you scroll down the table, you’ll also notice the ‘Status’ and ‘Comment’ data captured in separate rows.

### A note on writeback destinations

Customers using Inforiver must Bring Your Own Database (BYOD). This includes any database on-premise or in your private cloud, including shared folders such as OneDrive and SharePoint. This automatically ensures data security and data residency compliance. Inforiver does not offer any writeback destination databases or storage as part of the writeback service.

### CONCLUSION

In this tutorial, we learnt how to

1. **Write back values, text & comment data** from our Power BI matrix to Snowflake. The process is very similar for other destinations.
2. **Perform an unstructured writeback or a free-form writeback, where we did not have to create a database table in advance**
3. Control writeback options – including\
   (a) Writeback permissions to specific users\
   (b) Include totals or totals/subtotals during writeback\
   (c) Writeback only data with comments\
   (d) Write back a filtered data set\
   (e) Perform delta or full writeback\
   (f) Overwrite existing data or create new version each time\
   (g) … and more.

Interested to learn how you can roll out writeback capability to your users? [Reach out to us](https://inforiver.com/contact-us/) to learn more.

[Learn how Inforiver's writeback capability can transform your Power BI reports](https://inforiver.com/writeback-powerbi/).

\
