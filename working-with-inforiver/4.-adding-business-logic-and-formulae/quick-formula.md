# Quick formula

Inforiver provides several one-click calculations for inserting columns and rows.

### 1. Quick formula

Columns/measures such as running total, % contribution to parent/grand total etc. can be inserted in a single click. These options can be accessed from the Insert tab -> Quick formula in the toolbar.

<figure><img src="../../.gitbook/assets/4.5.1 Quick formula.png" alt=""><figcaption><p>Quick formula columns</p></figcaption></figure>

When you write custom formulas, you can also reference quick formula measures in them.

<figure><img src="../../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

#### i) Running total

The following configuration options are available for 'Running total'.&#x20;

Insert as - The running total can be inserted as a [measure or column](insert-manual-input-columns.md#2.-measure-vs-column).

Based on Measure - Column/measure based on which the running total needs to be calculated.

<figure><img src="../../.gitbook/assets/image (498).png" alt=""><figcaption><p>Running total for Actuals </p></figcaption></figure>

If you want to calculate the running total for all leaf nodes,  irrespective of the level of the hierarchy they belong to, select the 'Continuous Total'  checkbox.

<figure><img src="../../.gitbook/assets/image (499).png" alt=""><figcaption><p>Continuous running total for hierarchical datasets</p></figcaption></figure>

#### ii) Percentage running total

This formula is a variant of the running total quick formula. The running total is first calculated in the background at each level of the hierarchy after which it is displayed as a percentage of the total/subtotal.

<figure><img src="../../.gitbook/assets/image (500).png" alt=""><figcaption><p>Percentage running total formula</p></figcaption></figure>

#### iii) % Contribution to parent

In addition to choosing to insert as a visual measure/column and the base value, a progress bar can be enabled along with percentage and/or value to display.&#x20;

<figure><img src="../../.gitbook/assets/4.5.4(2) Quick formula.png" alt=""><figcaption><p>% Contribution of 2022 Actuals to parent</p></figcaption></figure>

#### iv) % Contribution to grand total

Contribution to the grand total can be inserted as shown below. To insert % contribution only for a selected category instead of all the categories or only for the column grand total, choose the 'Visual column' option and the corresponding column.&#x20;

<figure><img src="../../.gitbook/assets/4.5.5(2) Quick formula.png" alt=""><figcaption><p>% Contribution to grand total as visual column</p></figcaption></figure>

#### v) Lead/lag

You can perform a lead /lag calculation to shift any trend data by 'n' periods. This helps you quickly perform downstream variance calculations such as QoQ growth, YoY growth, etc. for each period.

<figure><img src="../../.gitbook/assets/4.5.6 Quick formula.png" alt=""><figcaption><p>Lead/lag calculations</p></figcaption></figure>

#### vi) Overall ranking

Ranks can be added across different groups in a single click. Choose to insert as a measure or column and the base measure. Note that there are no ranks applied for the subtotals.&#x20;

<figure><img src="../../.gitbook/assets/4.5.7 Quick formula.png" alt=""><figcaption><p>Overall ranking</p></figcaption></figure>

#### vii) Ranking within a group

Ranks within groups can be added including ranks for subtotals as shown in the below image.

<figure><img src="../../.gitbook/assets/4.5.8 Quick formula.png" alt=""><figcaption><p>Ranking within group</p></figcaption></figure>

#### viii) Insert variance

The default variance calculated by Inforiver is based on the first measure added to the AC/PY/PL/FC fields. _Insert Variance_ can be used to calculate the variance between any native measures or formula fields in your report.

<figure><img src="../../.gitbook/assets/image (305).png" alt=""><figcaption><p>Insert variance</p></figcaption></figure>

### 2. Smart analysis

% contribution and variance % columns can be added in a single click based on any cell in the visual. These can be accessed in the Insert tab -> Smart analysis as shown below.

{% hint style="info" %}
You need to select a cell to enable the 'Smart analysis' option.
{% endhint %}

<figure><img src="../../.gitbook/assets/4.5.9 Smart analysis.png" alt=""><figcaption><p>Smart analysis</p></figcaption></figure>

In the below image, % contribution has been added based on 2022 Actuals -> East.&#x20;

<figure><img src="../../.gitbook/assets/4.5.11(2) Smart analysis.png" alt=""><figcaption><p>Smart analysis - Contribution</p></figcaption></figure>

In the below image, % variance has been added based on the grand total. But you can choose any other value as well. Note that the calculation gets added as a measure or column based on the presence of categories in the column field.

<figure><img src="../../.gitbook/assets/4.5.10 Smart analysis.png" alt=""><figcaption><p>Smart analysis - Variance </p></figcaption></figure>

### 3. % Contribution rows

% Contribution based on any row can be inserted in a single click. To achieve this, in the Insert tab-> Insert row, select '% Contribution row'.

{% hint style="info" %}
Select a row to enable the 'Insert row' option.
{% endhint %}

<figure><img src="../../.gitbook/assets/4.5.12 Contribution row.png" alt=""><figcaption><p>% Contribution row</p></figcaption></figure>

The % contribution row gets added as shown below.

<figure><img src="../../.gitbook/assets/4.5.13 Contribution row.png" alt=""><figcaption><p>% Contribution row added</p></figcaption></figure>
