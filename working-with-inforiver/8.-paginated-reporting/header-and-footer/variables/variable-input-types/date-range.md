# Date Range

You can use the date range variable to choose a time frame or pick a single date.

### 1. Configuration

This section outlines configurations specific to date range variables.

**i) Format:** Inforiver supports a range of date formats which you can select from the dropdown. You can also set a custom format.

<figure><img src="../../../../../.gitbook/assets/image (445).png" alt=""><figcaption><p>Date format options</p></figcaption></figure>

**ii) Orientation:** You can choose whether to display the from date and to date in a single line(horizontal) or one below the other(vertical). The example shows date range variables arranged in horizontal and vertical orientations.

<figure><img src="../../../../../.gitbook/assets/image (446).png" alt=""><figcaption><p>Date range orientation</p></figcaption></figure>

**iii) Date label:** You can key in the name in the From and To textboxes to set custom labels.&#x20;

<figure><img src="../../../../../.gitbook/assets/image (447).png" alt=""><figcaption><p>Custom date label</p></figcaption></figure>

**iv) From date and To date:** Set the minimum and maximum date values that can be set  - the user will be able to select values that fall within the specified range.

**v) Disable Range:** Enable this option if you only need a single date picker and do not require a date range.&#x20;

<figure><img src="../../../../../.gitbook/assets/image (448).png" alt=""><figcaption><p>Disable range</p></figcaption></figure>

**vi) Select style:** Inforiver provides the flexibility to change the look and feel of a component with several built-in styles.

<figure><img src="../../../../../.gitbook/assets/image (449).png" alt=""><figcaption><p>Date range styles</p></figcaption></figure>

### 2. Examples

#### 2.1. Filter date values using date range

**STEP 1:** Create a date range variable and add a script to show the data between the specified start and end dates.

<figure><img src="../../../../../.gitbook/assets/image (8).png" alt=""><figcaption><p>Create a date range variable</p></figcaption></figure>

**STEP 2:** Use the date range variable to display data between the selected period.

<figure><img src="../../../../../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Date range variable</p></figcaption></figure>

#### 2.2. Relative date range filtering

You choose from predefined options like "last 7 days," "last month," "next quarter," etc. These filters automatically adjust based on the current date, ensuring that the report always reflects the desired time frame without manual intervention.

**STEP 1:** Create a date range variable and choose the relative date range template from the style selection section.

<figure><img src="../../../../../.gitbook/assets/image (1) (1) (1).png" alt=""><figcaption><p>Date range variable</p></figcaption></figure>

**STEP 2:** Create an Inforiver filter and use the variable created in the previous step as the filter parameter.

<figure><img src="../../../../../.gitbook/assets/image (1) (1) (1) (1).png" alt=""><figcaption><p>Create an Inforiver filter</p></figcaption></figure>

**STEP 3:** Use the variable date range filter to display data for periods relative to the current date.

<figure><img src="../../../../../.gitbook/assets/image (2) (1).png" alt=""><figcaption><p>Relative date filters</p></figcaption></figure>
