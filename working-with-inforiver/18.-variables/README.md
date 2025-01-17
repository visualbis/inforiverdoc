# 18. Variables

Analysts are often faced with the challenging task of navigating large datasets that span across multiple dimension categories and time frames - this is where Inforiver variables can save the day. Variables offer a range of options to efficiently traverse your datasets, apply filters, and even run ad-hoc scripts. Variables are graphical controls like buttons, checkboxes, or steppers that can accept user input to perform actions like setting a filter or changing the layout.&#x20;

See how variables can make report navigation and editing easier without creating Inforiver filters or manually editing the header or visual measures.

<figure><img src="../../.gitbook/assets/2.2. variables-gif.gif" alt=""><figcaption><p>Variable controls in Inforiver</p></figcaption></figure>

Let's take a deep dive into Inforiver variables.

## 1. Creating variables

**STEP 1:** You can create variable controls in your reports by clicking the **Variables** button in the **Insert** ribbon.

<figure><img src="../../.gitbook/assets/image (1168).png" alt=""><figcaption><p>Creating variables</p></figcaption></figure>

**STEP 2:** Click the **Add Variable** button in the **Define Variables** window. You'll need to specify the&#x20;

* **Label**: Set a name to identify the variable.
* **Type**: Choose the type of variable: numeric, options, text, button, boolean, date range, etc.
* **Value**: Set a default value for the variable.

<figure><img src="../../.gitbook/assets/image (1169).png" alt=""><figcaption><p>Different types of variables</p></figcaption></figure>

**STEP 3:** Click the edit<img src="../../.gitbook/assets/image (1170).png" alt="" data-size="line"> icon to customize the variable. We'll cover the various options in detail in subsequent sections.

<figure><img src="../../.gitbook/assets/image (1171).png" alt=""><figcaption><p>Variable properties</p></figcaption></figure>

**STEP 4:** You can display variables in a side panel. Check the **Include in Variables Panel** option if you want to expose the variable in the Variables panel. You can also provide a description of the variable's function.

<figure><img src="../../.gitbook/assets/image (1172).png" alt=""><figcaption><p>Include variable in panel</p></figcaption></figure>

After you create variables, the variables side pane is displayed from where users can input values for calculations, apply filters, and trigger scripts.

<figure><img src="../../.gitbook/assets/image (1175).png" alt=""><figcaption></figcaption></figure>

## 2. Referencing variables in functions

You can create a calculated measure that references the value set in a variable. Each variable has a **Technical Name** that can be referenced in formulas.

<figure><img src="../../.gitbook/assets/image (5).png" alt=""><figcaption><p>Technical name of the variable</p></figcaption></figure>

In this example, the calculated measure, Tax will change based on the toggle variable.

<figure><img src="../../.gitbook/assets/image (1176).png" alt=""><figcaption><p>Refercing the technical name is formulas</p></figcaption></figure>
