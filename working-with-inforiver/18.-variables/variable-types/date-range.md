# Date range

Use the date range variable in reports with date dimensions to select a period range.

### 1. Configuration <a href="#id-1.-configuration" id="id-1.-configuration"></a>

This section outlines configurations specific to date range variables.

**1.1. Value:** Assign a default date range for the variable.

**1.2. Enable date range:** Set a time frame within which the date range should be set. You can specify and start date that is lesser than the start date in the Value field and an end date that is greater than the end date in the Value field.

<figure><img src="../../../.gitbook/assets/image (3).png" alt=""><figcaption><p>Creating date range variables</p></figcaption></figure>

### 2. Examples <a href="#id-2.-examples" id="id-2.-examples"></a>

**2.1. Filter data**

When you have date dimensions in your reports, you can use date variables to create dynamic filters.

**STEP 1:** Create a date variable with the configuration shown in section 1.

**STEP 2:** Create an Inforiver filter that references the technical name of the date variable.

<figure><img src="../../../.gitbook/assets/image (1179).png" alt=""><figcaption><p>Create an Inforiver filter</p></figcaption></figure>

**STEP 3:** Notice how the data gets filtered as the variable selection is changed. The Inforiver filter needs to be created only once and does not have to be edited each time we change the date range.

<figure><img src="../../../.gitbook/assets/Untitled Project (15).gif" alt=""><figcaption><p>Filtering date based data using variables</p></figcaption></figure>
