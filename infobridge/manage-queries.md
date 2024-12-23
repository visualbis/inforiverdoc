# Manage queries

You can manage Infobridge queries by hovering over a query name to access the context menu. From there, you can duplicate, group, delete, or refresh the query.

<figure><img src="../.gitbook/assets/image (1088).png" alt=""><figcaption><p>Query management context menu</p></figcaption></figure>

### 1. Re-run

Re-executes the last step. In this example, we added two queries, so re-running the process will execute the append function again.

<figure><img src="../.gitbook/assets/image (1090).png" alt=""><figcaption></figcaption></figure>

### 2. Refresh

* **Refresh now**: Triggers a source refresh. If you've added new dimensions or measures or updated native measure values in your source, you can pull in the latest changes with this option.
* **Schedule refresh:** You can automate source refreshes by creating a schedule. Infobridge will trigger a refresh at the specified date and time.
* **Refresh history:** View the logs and milestones related to source refresh jobs.

[Learn more about managing sources](manage-sources.md).

<figure><img src="../.gitbook/assets/image (1091).png" alt=""><figcaption><p>Refresh options</p></figcaption></figure>

### 3. Duplicate

Use this option to create a copy or a backup of your query.

### 4. Copy identifier

Each bridge is assigned a unique identifier. You can use the identifier instead of the bridge name when you add a new Inforiver source report to a bridge. If you have 2 bridges with the same name, you can use the bridge identifier to distinguish between them.

### 5. Copy query GUID

The query GUID can be used to uniquely identify a particular query. The GUID is used when we need to lookup a value from a query without creating an integration. [Learn more about Infobridge lookups.](../formula-syntax/miscellaneous-functions/lookup.md)

### 6. Move to group

You can now group related data within Infobridge, allowing you to logically group your queries. Notice how the queries related to sales and profits have been grouped together.

<figure><img src="../.gitbook/assets/image (1092).png" alt=""><figcaption><p>Grouping queries</p></figcaption></figure>
