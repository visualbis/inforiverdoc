# Simulation slider

A slider variable can be used to pass a numeric or percentage value to a script or a filter.

### 1. Configuration

This section outlines configurations specific to simulation slider variables.

#### **i) Default value**

On initialization, the slider is set to the value specified in the default value textbox. By default, it is set to 0.

<figure><img src="../../../../../.gitbook/assets/image (437).png" alt=""><figcaption><p>Default value for simulation slider</p></figcaption></figure>

Notice how the slider is set at 5 on initialization, although the minimum value is 1.

<figure><img src="../../../../../.gitbook/assets/image (438).png" alt=""><figcaption><p>Slider set at default value</p></figcaption></figure>

#### **ii) Value as decimal**

The slider displays up to two decimal points when this option is enabled.

<figure><img src="../../../../../.gitbook/assets/image (439).png" alt=""><figcaption><p>Slider with decimal points enabled</p></figcaption></figure>

Notice how decimal places are displayed on the slider when the _Value as decimal_ property is enabled.

<figure><img src="../../../../../.gitbook/assets/image (440).png" alt=""><figcaption><p>Decimal points in slider</p></figcaption></figure>

#### **iii) Min and Max**

Set the minimum and maximum values that can be set in the slider - the user will be able to select values that fall within the specified range.

#### **iv) Scaling factor**&#x20;

Based on your data, you can set the scaling factor for the slider.

<figure><img src="../../../../../.gitbook/assets/image (462).png" alt=""><figcaption><p>Scaling factor</p></figcaption></figure>

When your dataset contains large values, setting an appropriate scaling factor enables you to filter your data easily. In the example below, the scaling factor has been set to None, making it difficult to read large values.

<figure><img src="../../../../../.gitbook/assets/image (466).png" alt=""><figcaption><p>Scaling factor set to None</p></figcaption></figure>

Setting the scaling factor to 'Millions' makes the values easier to gauge.

<figure><img src="../../../../../.gitbook/assets/image (467).png" alt=""><figcaption><p>Scaling factor in Millions</p></figcaption></figure>

#### **v) Value as percentage**

This option can be used in calculations involving percentages E.g., use a slider to calculate a percentage of profits

**vi)  Select style:** Inforiver provides the flexibility to change the look and feel of a component with several built-in styles.

<figure><img src="../../../../../.gitbook/assets/image (464).png" alt=""><figcaption><p>Slider styles</p></figcaption></figure>

### 2. Examples

#### a) Ranking with TopN/BottomN a numeric simulation slider

* Create a slider variable, and assign the min and max values for ranking. Create a script to accept the slider input to display the TopN categories.

{% hint style="info" %}
You can use a numeric stepper as well in this scenario.
{% endhint %}

<figure><img src="../../../../../.gitbook/assets/image (424).png" alt=""><figcaption><p>Simulation slider configuration for ranking</p></figcaption></figure>

* The value set in the slider will be used to display the top-performing or bottom-performing categories. In the example, we have used the slider variable to display the top 3 categories with the highest profit.&#x20;

<figure><img src="../../../../../.gitbook/assets/image (425).png" alt=""><figcaption><p>Using a slider to set TopN</p></figcaption></figure>
