# Button

You can use the button variable to trigger a set of actions such as setting the layout, ranking the data, or displaying data for a specific period.&#x20;

### 1. Configuration

The main configuration for a button is the list of actions to be performed on clicking.

**i) On Click:** You can use Inforiver's [built-in scripts ](../../../../../formula-syntax/scripting-functions/)to perform operations like showing or hiding a column or setting a conditional formatting rule.

<figure><img src="../../../../../.gitbook/assets/image (460).png" alt=""><figcaption><p>Triggering scripts with a button variable</p></figcaption></figure>

**ii) Select style:** Inforiver provides the flexibility to change the look and feel of a component with several built-in styles.

<figure><img src="../../../../../.gitbook/assets/image (461).png" alt=""><figcaption><p>Change button style</p></figcaption></figure>

### 2. Examples

#### &#x20;2.1. Trigger ad-hoc scripts using a button

**STEP 1:** Create a button variable, and add the scripts to change the layout to stepped, set a dark background, and display only 2023 data.

<figure><img src="../../../../../.gitbook/assets/image (469).png" alt=""><figcaption><p>Button to trigger scripts</p></figcaption></figure>

**STEP 2:** All the scripts are executed when the button is clicked.

<figure><img src="../../../../../.gitbook/assets/image (470).png" alt=""><figcaption><p>Script execution using button variable</p></figcaption></figure>

#### 2.2. Apply filters using a button

{% hint style="info" %}
If you have created filters in your report, you can instantly create a button variable that references them by navigating to Insert Variable > Filter using Button > Select the filter to be applied.
{% endhint %}

**STEP 1:** Create Inforiver filters which can be referenced in scripts.

<figure><img src="../../../../../.gitbook/assets/image (493).png" alt=""><figcaption><p>Create an Inforiver filter</p></figcaption></figure>

**STEP 2:** Create a variable button that contains a script referencing the filter defined in Step 1. You can also create a button to clear any applied filter using the [clear filter script](../../../../../formula-syntax/scripting-functions/setfilter.md#clearfilter).

<figure><img src="../../../../../.gitbook/assets/image (494).png" alt=""><figcaption><p>Create a button variable</p></figcaption></figure>

**STEP 3:** Use the buttons to apply filters on your data.

<figure><img src="../../../../../.gitbook/assets/image (495).png" alt=""><figcaption><p>Use buttons to apply filters</p></figcaption></figure>

#### &#x20;2.3. Export reports to PDF/Excel/Clipboard

You can create scripts to export reports using button controls.

{% hint style="info" %}
You can instantly create button variables for export to Excel/PDF/Clipboard by navigating to Insert Variable > Export.
{% endhint %}

**STEP 1:**  Create a button variable and use the EXPORT function to generate extracts to Excel/PDF or the clipboard.

<figure><img src="../../../../../.gitbook/assets/image (3) (1) (1).png" alt=""><figcaption><p>Create a button variable</p></figcaption></figure>

**STEP 2:** Use the button variables to export your report.

<figure><img src="../../../../../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Use button variables for exports</p></figcaption></figure>
