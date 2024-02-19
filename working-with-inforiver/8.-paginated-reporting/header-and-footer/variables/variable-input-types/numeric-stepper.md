# Numeric stepper

You can use the stepper variable to incrementally adjust a value within a predefined range. Stepper widgets are commonly used for selecting numeric values such as quantity, time, or any other parameter that can be adjusted in discrete steps.

### 1. Configuration

This section outlines configurations specific to stepper variables.

<figure><img src="../../../../../.gitbook/assets/image (441).png" alt=""><figcaption><p>Stepper configuration</p></figcaption></figure>

**i) Default value:** The slider is set to the value specified in the default value textbox. By default, it is set to 0.

**ii) Min and Max:** Set the minimum and maximum values that can be set in the stepper - the user will be able to select values that fall within the specified range.

**iii) Steps:** The increment between two consecutive values. For example, if Steps is 2 and the existing value is 4, then the next value in the stepper will be 6.

**iv) Scaling factor:** You can set the scaling factor based on your data. Setting an appropriate scaling factor enables you to filter and navigate your data easily.

**v)  Select style:** Inforiver provides the flexibility to change the look and feel of a component with several built-in styles.

<figure><img src="../../../../../.gitbook/assets/image (442).png" alt=""><figcaption><p>Stepper styles</p></figcaption></figure>

### 2. Use cases

#### &#x20;2.1. Traversing hierarchies using a stepper

**Step 1:** Create a stepper variable and configure the min/max range and the number of steps to increment with each click. Set up the script for navigating to a particular level of the hierarchy.

<figure><img src="../../../../../.gitbook/assets/image (426).png" alt=""><figcaption><p>Configuring a stepper variable</p></figcaption></figure>

**Step** **2**: Expand and collapse the hierarchy using the stepper. In the example, notice how the hierarchy has been expanded to 4 levels('0' refers to the highest level of the hierarchy).&#x20;

<figure><img src="../../../../../.gitbook/assets/image (427).png" alt=""><figcaption><p>Traversing the hierarchy using a stepper</p></figcaption></figure>

#### 2.2. Ranking using a stepper

You can display the top or bottom-performing categories using a stepper control.&#x20;

{% hint style="info" %}
Select the Ranking > TopN/BottomN/Both options from the Insert variable dropdown to directly create a stepper for TopN.
{% endhint %}

**Step 1:** Create a stepper variable and configure the min/max range and the number of steps to increment with each click. Set up the script for applying topN ranking based on the stepper value.



**Step 2:** Increment or decrement the stepper to rank the categories.
