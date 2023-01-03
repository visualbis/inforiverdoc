# Insert manual input columns

Inforiver provides six (6) different options to manually enter data in your Power BI report which are listed below.

| Input type | Description                                                                                               |
| ---------- | --------------------------------------------------------------------------------------------------------- |
| Number     | Double-click and start typing values in directly into a cell                                              |
| Text       | Enter text with multi-line support and word wrap                                                          |
| Dropdown   | Use the available presets or create your own list of values; supports both single-select and multi-select |
| Date       | Add a date from the calendar / date picker                                                                |
| Checkbox   |                                                                                                           |
| Person     | Input users from your organization (only available in Inforiver Enterprise)                               |

{% hint style="warning" %}
Inforiver Matrix offers only the first five types. There are certain other limitations in Inforiver Matrix that will be covered later in this section.&#x20;
{% endhint %}

a) If you are using the Enterprise version, you need to sign in as shown below.

<figure><img src="../../.gitbook/assets/4.4.0 Login.png" alt=""><figcaption><p>Sign in with Office 365 account</p></figcaption></figure>

b) Once you sign in successfully, your profile picture will be displayed as seen in the image.

<figure><img src="../../.gitbook/assets/4.4.1 Login.png" alt=""><figcaption><p>Sign in successful</p></figcaption></figure>

c) You can now start inserting a column to capture your data inputs by clicking on Insert --> Data Input.&#x20;

<figure><img src="../../.gitbook/assets/4.4.1 Data input.png" alt=""><figcaption><p>Data input columns</p></figcaption></figure>

## 1. Number

a) Select the 'Number' option in the dropdown.

<figure><img src="../../.gitbook/assets/4.4.3 Number.png" alt=""><figcaption><p>Inserting a numeric input column/measure</p></figcaption></figure>

b) By default, a visual measure gets inserted as shown below. There is a side panel which provides a number of customization options.

<figure><img src="../../.gitbook/assets/4.4.4 Number.png" alt=""><figcaption><p>Data input side panel</p></figcaption></figure>

c) The available properties are:

* **Insert as**: A column or measure can be inserted. If there is a column hierarchy, the input column is inserted for each category. In case of no column hierarchy, a single column is inserted.
* **Input type**: The type of data input column; can be changed from the initial selection before creating the column by clicking on 'Create'.&#x20;
* **Row aggregation type**: By default, totals and subtotals are defined as the sum of child rows. There are a number of other options such as average, minimum, maximum etc.&#x20;
* **Distribute parent value to children**: The values entered at a parent level are distributed to the child rows when enabled. This is very useful when creating budgets or forecasts.&#x20;
* **Allow input**: By default, inputs are enabled in both read and edit modes. But, based on your requirement, you can allow inputs only in edit mode or based on a formula.
* **Description**: Option to add a note for reference

d) Let's just change the title and go with the default for the other properties. Click 'Create'.

<figure><img src="../../.gitbook/assets/4.4.6 Number.png" alt=""><figcaption><p>Inserting a numeric measure</p></figcaption></figure>

e) The measure gets inserted. You can see that the column grand total also gets enabled.

<figure><img src="../../.gitbook/assets/4.4.7 Number.png" alt=""><figcaption><p>Numeric measure inserted</p></figcaption></figure>









## 2. Text







## 3. Dropdown



### i) Select



### ii) Multi-select





## 4. Checkbox





## 5. Date





## 6. Person







