# Enterprise features

As mentioned in [manual input columns](../insert-manual-input-columns.md), Inforiver Enterprise provides additional features compared to Inforiver Premium Matrix.

1. Data type - Person
2. Track changes at row level using the last updated at/by columns
3. List of values (LOV) from dimensions or other Power BI datasets

{% hint style="info" %}
You need to [sign in](../insert-manual-input-columns.md#1.-sign-in) to access the Enterprise features.
{% endhint %}

Let's take a detailed look.

## 1. Person

In the 'Data input' dropdown, you can now see an additional type called Person. Once a data input column is added in Inforiver Enterprise, two columns – Last updated at and last updated by get enabled. These are covered in [track changes at the row level](enterprise-features.md#2.-track-changes-at-row-level).

<figure><img src="../../../.gitbook/assets/4.4.4.2 Person.png" alt=""><figcaption><p>Data input column type - Person</p></figcaption></figure>

a) Click on 'Person'. The person column side panel is shown in the below image.&#x20;

You can choose to [insert as a visual measure or column](../insert-manual-input-columns.md#1.-insert-as). Entry can be enabled or disabled in the total/subtotal rows using the '[Allow entry on total/subtotal rows](dropdown.md#iii-entry-in-total-subtotal-rows)' checkbox. Input access can be configured using the '[Allow input](../insert-manual-input-columns.md#2.-allow-input)' option.&#x20;

Click 'Create'.

<figure><img src="../../../.gitbook/assets/4.4.4.4 Person.png" alt=""><figcaption><p>Person column properties</p></figcaption></figure>

b) The person column gets inserted. Double-click on any of the cells. You can see a list of the users within the organization. Select any of the users.

<figure><img src="../../../.gitbook/assets/4.4.4.5 Person.png" alt=""><figcaption><p>List of users</p></figcaption></figure>

c) Start typing a name or scroll to find the desired user. Click on the username.

<figure><img src="../../../.gitbook/assets/4.4.4.6 Person.png" alt=""><figcaption><p>Selecting a username</p></figcaption></figure>

d) You can also select multiple users if required.

<figure><img src="../../../.gitbook/assets/4.4.4.7 Person.png" alt=""><figcaption><p>Selecting multiple users</p></figcaption></figure>

e) Click 'Enter' to save the data. You can see the user's name displayed as shown below.

<figure><img src="../../../.gitbook/assets/4.4.4.8 Person.png" alt=""><figcaption><p>Person name captured</p></figcaption></figure>

## 2. Last updated at/by&#x20;

You can track changes at the row level using the two columns – 'Last updated at' and 'Last updated by' which capture metadata for changes in the data input columns.&#x20;

These are enabled once you add a data input column and can be found in the data input dropdown. Select/deselect to show/hide columns. They can also be enabled/disabled from the ‘Manage columns’ dropdown.

<figure><img src="../../../.gitbook/assets/4.4.4.1 Person.png" alt=""><figcaption><p>Last updated at/by columns</p></figcaption></figure>

## 3. List of values (LOV)

For the 'Single select' and 'Multi select' columns, a list of values (LOV) can be created from your Power BI datasets or from other dimensions like Master Data reference fields as shown in the below video.

{% embed url="https://lumel.wistia.com/medias/bppuqp940h" %}
List of values from Power BI datasets
{% endembed %}

Let's create a LOV from the datasets for a multi-select column.

a) In the multi-select column side panel, click on 'Datasets'.

<figure><img src="../../../.gitbook/assets/4.4.4.9 LOV.png" alt=""><figcaption><p>Datasets option</p></figcaption></figure>

b) You can see a dialog box as shown below.&#x20;

<figure><img src="../../../.gitbook/assets/4.4.4.10 LOV.png" alt=""><figcaption><p>Add options from datasets window</p></figcaption></figure>

c) You can select the Power BI workspace from the 'Workspace' dropdown.

<figure><img src="../../../.gitbook/assets/4.4.4.11 LOV.png" alt=""><figcaption><p>Workspace selection</p></figcaption></figure>

d) The datasets available in the selected workspace are auto populated. You can select the desired dataset from the dropdown.&#x20;

<figure><img src="../../../.gitbook/assets/4.4.4.12 LOV.png" alt=""><figcaption><p>Dataset selection</p></figcaption></figure>

e) Select the table from the 'Table' dropdown.

<figure><img src="../../../.gitbook/assets/4.4.4.13 LOV.png" alt=""><figcaption><p>Table selection</p></figcaption></figure>

f) All the columns available in the table are listed. You can select the column based on which the LOV is to be created.

<figure><img src="../../../.gitbook/assets/4.4.4.14 LOV.png" alt=""><figcaption><p>Column selection</p></figcaption></figure>

g) The unique elements in the selected column are listed as options. You can select all of them or unselect those that are not required. Click 'Apply'.&#x20;

<figure><img src="../../../.gitbook/assets/4.4.4.15 LOV.png" alt=""><figcaption><p>LOV created</p></figcaption></figure>

h) The selected options are displayed in the side panel as shown below. Click 'Create'.

<figure><img src="../../../.gitbook/assets/4.4.4.16 LOV.png" alt=""><figcaption><p>LOV created</p></figcaption></figure>

i) Double-click on a cell in the multi-select column. Select the options as required and press 'Enter'.

<figure><img src="../../../.gitbook/assets/4.4.4.17 LOV (1).png" alt=""><figcaption><p>Using the dropdown</p></figcaption></figure>

j) The selections are displayed as shown in the below image.

<figure><img src="../../../.gitbook/assets/4.4.4.18 LOV.png" alt=""><figcaption><p>Multi-select column</p></figcaption></figure>

In the next section, we'll be covering [quick formulas](../quick-formula.md).
