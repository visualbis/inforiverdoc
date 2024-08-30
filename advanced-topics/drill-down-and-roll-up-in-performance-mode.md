# Drill down and roll up in performance mode

Businesses often have hierarchical structures, such as organizational charts, product hierarchies, or geographical hierarchies. Navigating complex hierarchical data is an essential aspect of BI reporting – users should be able to drill down into more detailed information or drill up to view higher-level summaries. The et’s see how we can use Inforiver to navigate hierarchical structures and gain insights at different levels of granularity.

The performance mode in Inforiver has been designed to process large hierarchical datasets of more than 100k cells. However, in performance mode, you cannot access the full set of features provided by Inforiver. Certain features like pagination, Row, Column, Section Breaks, and Report+ are not supported.

{% hint style="info" %}
* Performance mode is available only in the Inforiver Reporting Matrix.
{% endhint %}



To enable drill down, we first need to activate the ‘Performance mode.’

<figure><img src="../.gitbook/assets/0 Toolbar performance mode enabled.png" alt=""><figcaption><p>Toolbar - performance mode activated</p></figcaption></figure>

{% hint style="warning" %}
When the performance mode is enabled or disabled, all changes like formatting or filters will be reset, and the report will be restored to the default configuration.
{% endhint %}

In the image below, we have a four-level hierarchy in the rows. You will be able to see drill down/roll up icons on the visual when performance mode is enabled.

<figure><img src="../.gitbook/assets/1. Performance mode.png" alt=""><figcaption><p>Hierarchical dataset with drill down/ roll up buttons enabled</p></figcaption></figure>

Let’s take a look at the drill-down/ roll-up operations in detail.&#x20;

#### 1. Drill up

The roll-up button can be used to navigate to the immediate upper level of the hierarchy, i.e., the parent level of the currently expanded level. To demonstrate this, we have used the roll-up icon to navigate from the ‘Segment’ level to the ‘Sub-category’ level. &#x20;

<figure><img src="../.gitbook/assets/4. Roll up.gif" alt=""><figcaption><p>Drill up</p></figcaption></figure>

#### 2. Drill down

Enable the drill-down mode to select and expand a particular node in the hierarchy. Only the immediate parent and children of the selected node will be displayed, while the rest of the hierarchy is hidden. To see this feature in action, let’s turn on drill down and select the ‘Accessories’ row.&#x20;

<figure><img src="../.gitbook/assets/5. Drill down.gif" alt=""><figcaption><p>Drill down</p></figcaption></figure>

#### 3. Drill down to the next level &#x20;

You can traverse the hierarchy level-by-level using this button. Only the child nodes belonging to a particular level of the hierarchy will be displayed. In the example, notice how all the child nodes for the ‘Furniture,’ ‘Office Supplies,’ and ‘Technology’ categories are displayed on drilling down. When we click the button again, the child nodes under level 3 of the hierarchy are displayed, i.e., the segment level. &#x20;

<figure><img src="../.gitbook/assets/6. Drill down next level.gif" alt=""><figcaption><p>Drill down next level</p></figcaption></figure>

#### 4. Expand one level&#x20;

You can expand the hierarchy to the next level and display the child nodes using this option. With each click, you can traverse the entire hierarchy, level by level.&#x20;

<figure><img src="../.gitbook/assets/7. Expand.gif" alt=""><figcaption><p>Expand one level</p></figcaption></figure>

Inforiver offers advanced support for hierarchical data structures which we will be covering in the upcoming sections.
