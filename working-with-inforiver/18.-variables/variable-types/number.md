# Number

Create number variables when you need to pass a numeric or percentage value to a script or a filter.

### 1. Configuration <a href="#id-1.-configuration" id="id-1.-configuration"></a>

This section outlines configurations specific to number variables.

**1.1. Value:** Assign a default value for the number variable.&#x20;

**1.2. Value as percentage:** Enable this option if the variable will be used in calculations involving percentages E.g., calculate a percentage of profits.

**1.3. Show as slider:** A numeric slider will be displayed instead of a textbox.

**1.4. Min and Max:** Set the minimum and maximum values that can be set in the slider - the user will be able to select values that fall within the specified range.

<figure><img src="../../../.gitbook/assets/image (3) (1) (1) (1) (1) (2) (1).png" alt=""><figcaption><p>Number variable configurations</p></figcaption></figure>

### 2. Examples <a href="#id-2.-examples" id="id-2.-examples"></a>

#### **2.1. Pass values dynamically to formulae**

**STEP 1:** Create a numeric variable with the configuration shown below.

<figure><img src="../../../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (2) (1) (1) (1).png" alt=""><figcaption><p>Create a numeric slider variable</p></figcaption></figure>

**STEP 2:** Create a calculated measure and reference the technical name of the slider variable in the formula.

<figure><img src="../../../.gitbook/assets/image (2) (1) (1) (1) (1) (1) (3) (1) (1).png" alt=""><figcaption><p>Create calculated measure </p></figcaption></figure>

**STEP 3:** Calibrate the slider to view the interest paid at varying interest rates.

<figure><img src="../../../.gitbook/assets/Untitled Project (2).gif" alt=""><figcaption><p>Numeric slider in action</p></figcaption></figure>

#### **2.2. Dynamically filter data**&#x20;

**STEP 1:** Create a numeric variable with the configuration shown below.

<figure><img src="../../../.gitbook/assets/image (3) (1) (1) (1) (1) (2) (1) (1).png" alt=""><figcaption><p>Create numeric variable</p></figcaption></figure>

**STEP 2:** Create an Inforiver filter that references the technical name of the numeric variable.

<figure><img src="../../../.gitbook/assets/image (4) (14).png" alt=""><figcaption><p>Create a Filter</p></figcaption></figure>

**STEP 3:** Enter values in the variable and notice how the data gets filtered on the fly without having to update the Inforiver filter each time.

<figure><img src="../../../.gitbook/assets/Untitled Project (14).gif" alt=""><figcaption><p>Filtering data with a numeric variable</p></figcaption></figure>
