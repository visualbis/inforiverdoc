# Manage rules

When you have several conditional formatting rules in your report, you can easily view and modify them using the 'Manage rules' option.&#x20;

To access, click on the Conditional formatting dropdown and select 'Manage rules' as shown in the below image. A side panel opens showing a list of all the rules.

<figure><img src="../../.gitbook/assets/Manage Rules.png" alt=""><figcaption><p>Manage rules side panel</p></figcaption></figure>

a) To edit the existing rules, click on the **Pencil** icon.

b) You can use the **Duplicate** icon to create a copy of existing rules and edit further as required.

c) You can delete the rules using the **Delete** icon corresponding to that rule.

d) Using the **On/off toggle**, you can enable/disable the rules.

e) You can reorder and prioritize the rules using the gripper to drag and drop rules.

{% hint style="info" %}
You cannot duplicate conditional formatting types such as quick rules, heat maps, and classifications.
{% endhint %}

#### Prioritizing rules

Let's consider an example of prioritizing rules. Let's add two rules as defined below.

Rule 1: When 2022 Actuals < 2022 Plan, 2022 Actuals are shown in red.

Rule 2: When 2022 Actuals < 2021 Actuals, 2022 Actuals are shown in blue.

When 2022 Actuals are lesser than both the 2022 Plan and 2021 Actuals, there is a conflict. In such cases, the first rule in the order is executed.&#x20;

In the image on the left, Rule 1 is executed first. So, the highlighted values are in red. In the image on the right, the same values are in blue.

<div>

<figure><img src="../../.gitbook/assets/CF1 (1).png" alt=""><figcaption><p>AC &#x3C; PL has a higher priority</p></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/CF2 (1).png" alt=""><figcaption><p>AC &#x3C; PY has a higher priority</p></figcaption></figure>

</div>

In the next section, we'll be covering [customization options in charts](../6.-working-with-charts.md).
