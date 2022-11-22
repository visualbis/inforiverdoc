# Basic interactions

## Top n

In this document, let us get to know how the **Top n** feature works in Inforiver. **Top n** deals with classifying the Top and Bottom categories based on the measures.&#x20;

**Top n** can be applied to only **one column/measure** at a time. Though, you can add multiple Top or Bottom n conditions on the same measure.

Let us see about the **Top n** functionality in detail below.

Consider the example of displaying the Top 5 City Sales Value (2016 Sales) in each Subcategory.

* Select the **Sales** (2016 Sales) column/measure.
* Click **Home** from the toolbar and select **Top n** from the **Analyze** section.

<figure><img src="../.gitbook/assets/TopN.png" alt=""><figcaption><p>Top n </p></figcaption></figure>

*   In the **Top n** dialog box that appears, input the following fields:

    * Top/Bottom/Both: Both displays Top and Bottom values **(Top)**
    * Number of items **(5)**
    * Condition-based on Value or Percentage **(Value)**
    * Field to which condition to be applied **(Sub-Category)**



    <figure><img src="../.gitbook/assets/Choose.png" alt=""><figcaption><p>Choose from Top, Bottom or Both</p></figcaption></figure>


* To display the remaining categories as **Others**, check the respective checkbox. Inorder to customize the name “**Others**”, click on the **Pen** icon.

<figure><img src="../.gitbook/assets/Others.png" alt=""><figcaption><p>Aggregate the Rest as Others</p></figcaption></figure>

* Check “**Suffix Others with category name**”, to display the category label along with Others.

<figure><img src="../.gitbook/assets/Suffix.png" alt=""><figcaption><p>Show the category label as suffix</p></figcaption></figure>

* Click **Apply**, the result is shown below.

<figure><img src="../.gitbook/assets/Top 5.png" alt=""><figcaption><p>Top 5 Subcategory based on the Value</p></figcaption></figure>

* To apply another **Top n** condition, follow the same procedure as illustrated above.
* In the **Top n** dialog box, click on **Add rule**.
* Select the fields as shown in the below image:

<figure><img src="../.gitbook/assets/Add Rule.png" alt=""><figcaption><p>Add Rule</p></figcaption></figure>

<figure><img src="../.gitbook/assets/Result (2).png" alt=""><figcaption><p>Showing result with added rule</p></figcaption></figure>

* To delete a **Top n** condition, click on the respective **Delete** icon.

<figure><img src="../.gitbook/assets/Delete.png" alt=""><figcaption><p>Delete</p></figcaption></figure>

* To clear all the **Top n** conditions, click on **Reset All** Button.

<figure><img src="../.gitbook/assets/Reset (1).png" alt=""><figcaption><p>Reset all</p></figcaption></figure>

* The following warning message gets displayed when you try to apply **Top n** on another column/measure simultaneously.

<figure><img src="../.gitbook/assets/warning.png" alt=""><figcaption><p>Warning Message</p></figcaption></figure>

