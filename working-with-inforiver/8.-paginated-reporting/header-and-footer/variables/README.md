# Variables

Analysts are often faced with the challenging task of navigating large datasets that span across multiple dimension categories and time frames - this is where Inforiver variables can save the day. Variables offer a range of options to efficiently traverse your datasets, apply filters, and even run ad-hoc scripts. Variables are graphical controls like buttons, checkboxes, or steppers that can be used to perform actions like setting a filter or changing the layout. You can add and configure variables in the header section of your reports. Variables can be used with other types like charts, text, and KPIs to design the header. Let's take a deep dive into Inforiver variables.

## 1. Adding a variable to the header

There are two ways to insert variables in your reports:

#### i) Insert tab

You can create a variable from the Insert ribbon. Selecting the _**Insert New Variable**_ option will open the Edit Variables side pane from where you can configure the variable.

<figure><img src="../../../../.gitbook/assets/image (420).png" alt=""><figcaption><p>Creating a variable from the insert tab</p></figcaption></figure>

#### ii) Header and footer tab

Navigate to the Design > Header & Footer ribbon. You can insert the variables either from the Type dropdown or by clicking on the Insert Variables button.

{% hint style="info" %}
One header container can support only one variable. To create additional variables, you need to [split the container](../../header-and-footer.md#id-2.-basic-interactions) or add a new row or column.
{% endhint %}

<figure><img src="../../../../.gitbook/assets/image (421).png" alt=""><figcaption><p>Creating variables from the Insert ribbon</p></figcaption></figure>

## 2. Configuring variables

The Edit Variables side pane opens when you add a new variable. Let's look at the configuration options for variables.

<figure><img src="../../../../.gitbook/assets/image (422).png" alt=""><figcaption><p>Edit variables side pane</p></figcaption></figure>

**i) Name**: A user-defined name to uniquely identify the variable.&#x20;

**ii) Input type:** The type of graphical control to be used to trigger an action like setting a filter or hiding a row/column. [Learn more about the different input types available in Inforiver.](variable-input-types/)

<figure><img src="../../../../.gitbook/assets/image (423).png" alt=""><figcaption><p>Input type dropdown</p></figcaption></figure>

**iii) Disable editing in read view:** When this option is enabled, report viewers will not be able to change the variables, they can only view the configurations that have been set by the creator.

<figure><img src="../../../../.gitbook/assets/image (472).png" alt=""><figcaption><p>Disable editing in read view option</p></figcaption></figure>

Report users will be able to view the variable setup in reading mode.

<figure><img src="../../../../.gitbook/assets/image (473).png" alt=""><figcaption><p>Reading view for variables</p></figcaption></figure>

**iv) Show label:** You can set custom labels for variables. Enable the _Show Label_ option to display a custom name.

<figure><img src="../../../../.gitbook/assets/image (474).png" alt=""><figcaption><p>Show label</p></figcaption></figure>

**v) On change:** You can execute scripts when the state of a variable changes, for example, when a button is clicked, an option is selected or a toggle switch is turned off. Inforiver provides a range of built-in scripts that you can use. [Learn more about scripting functions.](../../../../formula-syntax/scripting-functions/)

<figure><img src="../../../../.gitbook/assets/image (475).png" alt=""><figcaption><p>Execute scripts</p></figcaption></figure>

**vi) Description:**  Provide details for the variable.

<figure><img src="../../../../.gitbook/assets/image (476).png" alt=""><figcaption><p>Variable description</p></figcaption></figure>

## 3. Referencing variables in functions

You can create a calculated measure that references the value set in a variable. The reserved keyword 'VARIABLES' can be used to list all the variables in your report. You can then select the variable required for your formula.

<figure><img src="../../../../.gitbook/assets/image (477).png" alt=""><figcaption><p>Referencing variable values in functions</p></figcaption></figure>

## 4. Pre-configured variables

Inforiver has pre-built variables that you can instantly add to your reports. You can choose the variable from the Insert variable dropdown and Inforiver will internally configure them based on the categories or measures in your dataset. For instance, if you add a "Go to Level - Rows" variable, Inforiver will create a dropdown listing the row categories. When you select a particular category from the dropdown, only that level of the hierarchy will be displayed.

<figure><img src="../../../../.gitbook/assets/Untitled Project.gif" alt=""><figcaption><p>Using pre-configured variable options</p></figcaption></figure>
