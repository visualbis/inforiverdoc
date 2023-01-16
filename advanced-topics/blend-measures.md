# Blend measures

Inforiver allows you to blend two measures in a single column along with formatting, including conditional formatting.&#x20;

Let's blend the Sales and Margin% columns in a single column.&#x20;

a) In the 'Insert' tab, click on the 'Blend' option in the 'Column' section. A blank measure gets inserted and the 'Blend measure' side panel opens.&#x20;

<figure><img src="../.gitbook/assets/Blend measure.png" alt=""><figcaption><p>Blend</p></figcaption></figure>

b) Enter the title and select the measures as shown from the dropdown. Click 'Create'.

<figure><img src="../.gitbook/assets/a.1.1 Blend.png" alt=""><figcaption><p>Blend measure panel</p></figcaption></figure>

c) The columns are blended to create a single column. Note that Margin % is displayed below Sales. This is because we have used the default 'Vertical' as 'Blend direction'.

<figure><img src="../.gitbook/assets/Blend vertically.png" alt=""><figcaption><p>Blend measures vertically</p></figcaption></figure>

d) If you want to display in a horizontal orientation, change the 'Blend direction' to 'Horizontal' and click 'update'.

<figure><img src="../.gitbook/assets/Blend Horizontal.png" alt=""><figcaption><p>Blend measures horizontally</p></figcaption></figure>

e) The horizontal blending is shown.

<figure><img src="../.gitbook/assets/Horizontal blen.png" alt=""><figcaption><p>Horizontal blending</p></figcaption></figure>

f) The other way to blend the columns is by selecting the columns to be combined and clicking the 'Blend' option from the Insert tab. For example, let's blend the Margin and Margin% columns in a single column.&#x20;

Select the columns and click 'Blend'.

<figure><img src="../.gitbook/assets/Blend Measures2.png" alt=""><figcaption><p>Blend by selecting columns</p></figcaption></figure>

g) The 'Blend measure' side panel opens, enter the title and click 'Create'.

<figure><img src="../.gitbook/assets/a.1.2 Blend.png" alt=""><figcaption><p>Blend measure panel</p></figcaption></figure>

h) The columns are blended into a single column.

<figure><img src="../.gitbook/assets/Margin and Margin%.png" alt=""><figcaption><p>Blended column</p></figcaption></figure>

i) If you want to view only the blended columns, click on 'Manage Columns' from the toolbar. You can see a list showing the row and column headers and measures.

<figure><img src="../.gitbook/assets/Manage Columns.png" alt=""><figcaption><p>Manage columns</p></figcaption></figure>

j) Unselect the original source columns which you want to hide in the visual. You can now see only the blended columns.

<figure><img src="../.gitbook/assets/Unselect the column.png" alt=""><figcaption><p>Hiding source columns</p></figcaption></figure>

{% hint style="info" %}
When two columns are blended, the formatting of the source columns including conditional formatting is retained in the new merged column. &#x20;
{% endhint %}

**Example 1:** Consider an example where the font style and size are changed in the source columns.

a) Let's change the font style to bold for the 'Sales' column. You can see that the same style has been copied to the Sales values of the merged column (Sales| Margin %).

<figure><img src="../.gitbook/assets/Bold.png" alt=""><figcaption><p>Blend font style</p></figcaption></figure>

b) Let's keep the 'Sales' as it is and reduce the font size of the 'Margin %' column.

<figure><img src="../.gitbook/assets/Font size (2).png" alt=""><figcaption><p>Formatting font size</p></figcaption></figure>

c) You can see that the values in the merged columns reflect the change.

<figure><img src="../.gitbook/assets/Blend format size.png" alt=""><figcaption><p>Blend font size</p></figcaption></figure>

**Example 2:** Consider the below example where conditional formatting is applied to the 'Sales' column.&#x20;

a) To view the conditional formatting rule, in the 'Home' tab, click on the 'Conditional formatting' drop-down and select 'Manage rules'.&#x20;

<figure><img src="../.gitbook/assets/CF (1).png" alt=""><figcaption><p>Manage rules</p></figcaption></figure>

b) A side panel opens showing a list of all the rules. Click on the 'Edit' icon next to the rule Icons - Margin %.

<figure><img src="../.gitbook/assets/edit cf.png" alt=""><figcaption><p>Conditional formatting panel</p></figcaption></figure>

c) Let's try changing the icon position and see what happens to the source and merged columns.

<figure><img src="../.gitbook/assets/Icon pos.png" alt=""><figcaption><p>Icon position</p></figcaption></figure>

d) When you change the icon position from 'Right of data' to 'Left of data' and select 'Apply', you can see that the icons in both columns shift over.&#x20;

<figure><img src="../.gitbook/assets/Blend Cf.png" alt=""><figcaption><p>Blend conditional formatting</p></figcaption></figure>

**Example 3:** Let's see how to blend the two measures in a single column with data bars. Follow the steps shown below:

a)  Select the columns and click 'Blend'.

<figure><img src="../.gitbook/assets/Blend Data bars.png" alt=""><figcaption><p>Data bars</p></figcaption></figure>

b) The 'Blend measure' side panel opens, enter the title and click 'Create'.

<figure><img src="../.gitbook/assets/Data bars.png" alt=""><figcaption><p>Blend measure panel</p></figcaption></figure>

c) You can see the two values along with the data bars in a single column.

<figure><img src="../.gitbook/assets/Blended bars.png" alt=""><figcaption><p>Blended data bars</p></figcaption></figure>
