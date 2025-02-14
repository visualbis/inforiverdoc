# Manage inserted rows

Rows inserted in the visual such as calculations, static rows, template rows, or data input rows can be managed using the **Manage Rows** option.&#x20;

## 1. Rows

Inserted rows such as static, calculated, etc. can be managed from the **Rows** tab. A list of the inserted rows is displayed. Each type of row: calculated, aggregated, data input, and template can be identified by the row icons. The following operations can be performed:

a) Edit - Formulae or other properties can be modified.

b) Delete - The inserted row can be permanently deleted.

c) Show/hide row - Inserted rows can be hidden temporarily.

d) Show/hide row indicator - The pencil icon beside the inserted rows can be hidden.

e) Add rows - You can instantly add child rows and sibling(at the same level of the hierarchy) rows right from the Manage Rows side pane.

Hover over the row to view these options.

<figure><img src="../../.gitbook/assets/image (1225).png" alt=""><figcaption><p>Row management operations</p></figcaption></figure>

f) Search and filter custom rows - Use the Search and Filter options to search for a particular row category or display rows based on the type.

<figure><img src="../../.gitbook/assets/image (1226).png" alt=""><figcaption><p>Search and filter for custom rows</p></figcaption></figure>

#### **Tree view**

Use the Tree View to easily identify the hierarchy level where a specific row was created.

<figure><img src="../../.gitbook/assets/image (1223).png" alt=""><figcaption><p>Tree view</p></figcaption></figure>

#### **List view**

The **List** view displays rows in the order in which they were inserted.

<figure><img src="../../.gitbook/assets/image (1224).png" alt=""><figcaption><p>List view</p></figcaption></figure>

## 2. Row settings

The **Manage Rows** side panel has a **Row Settings** tab that lets you configure settings such as user permissions.

### 2.1. Insert row configuration

You can set category-based rules on rows that are bulk-inserted. For example, you can disable row insertion for certain row dimension categories, enforce distinct values, or source categories from an Excel spreadsheet. [Learn more about bulk inserting rows.](insert-manual-input-rows.md#id-2.-bulk-insert-static-rows)

### 2.2. Insert Row Access

You can explicitly set permissions for users to insert rows in read mode. You have options to restrict all users, allow all users, or authorize specific users to insert rows. Navigate to Insert > Manage Rows >Settings > Insert Row Access to set permissions.

* Enable the **Allow in Read Mode** toggle to allow users to insert rows in reading mode.
* To allow all the members in your organization to insert rows, choose the **All users** radio button.
* If you want to restrict users from inserting rows, choose the **Specific users** radio butto&#x6E;**.** You will then be able select the users to whom you want to provide access.

<figure><img src="../../.gitbook/assets/4.8. Data input insert rows access 5.png" alt=""><figcaption><p>Insert row permissions</p></figcaption></figure>

### 2.3. Row edit user validation

You can set row-level permissions to edit rows of Data Input and Forecast columns. If your semantic model contains an Email ID field, you can grant access to specific email IDs to edit associated row categories. The steps to configure row edit access have been outlined below.

**STEP 1:** Specify the workspace, semantic model, table, and the field in the table that contains email IDs.

<figure><img src="../../.gitbook/assets/image (7) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Select table and email ID field</p></figcaption></figure>

**STEP 2:** Select the **All** radio button to set row edit permissions for all the forecasts and data input fields in your report. To grant access to specific measures, check the **Selected** radio button and choose the measure.

<figure><img src="../../.gitbook/assets/image (3) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Select measures to grant access</p></figcaption></figure>

**STEP 3:** Specify users who will have elevated access to edit all rows, irrespective of the categories assigned to email IDs in the semantic model.

<figure><img src="../../.gitbook/assets/image (4) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>User selection for elevated edit access</p></figcaption></figure>

**STEP 4:** Map the dimension category in the semantic model to the row dimension category in your report. Click **Save & Preview**.

<figure><img src="../../.gitbook/assets/image (7) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Map semantic model dimension to visual dimension</p></figcaption></figure>

**STEP 5:** Verify the email IDs and the categories assigned.

<figure><img src="../../.gitbook/assets/image (6) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Verify categories assigned</p></figcaption></figure>

Once row-level user edit validation is configured, users in read-only mode will only be able to modify the values for row dimension categories to which they have been granted access.
