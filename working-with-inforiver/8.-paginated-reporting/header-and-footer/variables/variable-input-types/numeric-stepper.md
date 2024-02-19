# Numeric stepper

You can use the stepper variable to incrementally adjust a value within a predefined range. Stepper widgets are commonly used for selecting numeric values such as quantity, time, or any other parameter that can be adjusted in discrete steps.

### 1. Configuration

This section outlines configurations specific to stepper variables.

<figure><img src="../../../../../.gitbook/assets/image (441).png" alt=""><figcaption><p>Stepper configuration</p></figcaption></figure>

**i) Default value:** The slider is set to the value specified in the default value textbox. By default, it is set to 0.

**ii) Min and Max:** Set the minimum and maximum values that can be set in the stepper - the user will be able to select values that fall within the specified range.

**iii) Steps:** The increment between two consecutive values. For example, if Steps is 2 and the existing value is 4, then the next value in the stepper will be 6.

**iv) Scaling factor:** Based on your data, you can [set the scaling factor](simulation-slider.md#iv-scaling-factor). Setting an appropriate scaling factor enables you to easily filter and navigate your data.

**v)  Select style:** Inforiver provides the flexibility to change the look and feel of a component with several built-in styles.

<figure><img src="../../../../../.gitbook/assets/image (442).png" alt=""><figcaption><p>Stepper styles</p></figcaption></figure>

### 2. Use cases

#### &#x20;a) Traversing hierarchies using a stepper

* Create a stepper variable and configure the min/max range and the number of steps to increment with each click. Set up the script for navigating to a particular level of the hierarchy.

<figure><img src="../../../../../.gitbook/assets/image (426).png" alt=""><figcaption><p>Configuring a stepper variable</p></figcaption></figure>

* Expand and collapse the hierarchy using the stepper. In the example, notice how the hierarchy has been expanded to 4 levels('0' refers to the highest level of the hierarchy).&#x20;

<figure><img src="../../../../../.gitbook/assets/image (427).png" alt=""><figcaption><p>Traversing the hierarchy using a stepper</p></figcaption></figure>
