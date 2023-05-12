# Scenarios (Enterprise only)

Inforiver Enterprise offers the ability to create new scenarios in edit and read modes based on an existing series for ad-hoc analysis. Once a scenario is created, you can either simulate or perform allocations on the native measures.

Scenarios are interactive and can be edited unless it’s explicitly locked. They can be created in both reading and edit mode and can be shared with other users. You can writeback all or specific scenarios and enable automatic writeback if required.

## 1. Create a scenario

{% hint style="info" %}
To create a scenario you need to log in with your Microsoft 365 account
{% endhint %}

You can create a new scenario by clicking the 'Create scenario' button under the 'Insert' tab of the Inforiver toolbar.

<figure><img src="../../.gitbook/assets/create-scenario.png" alt=""><figcaption><p>Create scenario option</p></figcaption></figure>

Clicking this option will open up a 'Create scenario' modal. This modal has a general tab and a permissions tab.

{% hint style="info" %}
The general and permission settings can be edited later after the creation
{% endhint %}

### i) General

Under the 'General' tab, you can configure the general scenario options and properties. You will find the following two options under this tab:

<figure><img src="../../.gitbook/assets/create-scenario (1).png" alt=""><figcaption></figcaption></figure>

**Scenario name** - In this input field, you can specify the name of the scenario

**Include series in scenario** -This field by default has all the metrics added. You can however add or exclude the series you want in your scenario.

**Start period and End period** - Here you can specify the starting and ending periods of the scenario

### ii) Permission

Under the 'Permission' tab, you can configure the scenario permissions.&#x20;

<figure><img src="../../.gitbook/assets/create-scenario-permission.png" alt=""><figcaption></figcaption></figure>

In the **Who can share the scenario** section, you can see the following two options:

**i) All users within your company domain** - If this option is selected, then all the users within your company domain will be able to share the created scenario

**ii) Specific users within your company domain** - Selecting this option will allow only the specified users to share the created scenario. If this option is selected, the 'Add users' input field becomes available. You can specify the email id of the people who can share this scenario in this input field.

<figure><img src="../../.gitbook/assets/create-scenario-permission-adduser.png" alt=""><figcaption></figcaption></figure>

Once all the permissions and settings are configured, click 'Create' to create a scenario.

## 2. Create a scenario in reading view mode

Creating a scenario in reading view mode follows the same procedure as the edit mode.&#x20;

But there is one additional step, you need to enable the 'Scenario tab' in the 'Reading view access' modal. You can learn more about configuring the reading view access modal [here](https://docs.inforiver.com/working-with-inforiver/3.-basic-interactions/actions/toolbar-options#6.-set-reading-view-access).

<figure><img src="../../.gitbook/assets/scenario-tab-option.png" alt=""><figcaption><p>Enable scenario tab in reading view mode</p></figcaption></figure>

## 3. Configure scenario

If a new scenario is successfully created, you will see a 'Scenario' tab in the Inforiver toolbar.

<figure><img src="../../.gitbook/assets/scenario-options.png" alt=""><figcaption><p>Scenario tab</p></figcaption></figure>

The scenario tab has the following options to configure the scenario-related settings:

### i) Create scenario

This option lets you create a new scenario. Clicking on this option will open up the 'Create scenario' modal. You can learn more about how to create a scenario [here](scenarios-enterprise-only.md#1.-create-a-scenario).

<figure><img src="../../.gitbook/assets/create-scenario-2.png" alt=""><figcaption><p>Create scenario option</p></figcaption></figure>

Alternatively, you can click the '+' icon next to your current scenario tab to create a new scenario.

<figure><img src="../../.gitbook/assets/create-scenario-3.png" alt=""><figcaption><p>Create scenario icon option</p></figcaption></figure>

### ii) Scenario settings

This option lets you edit the previously configured scenario settings. Clicking this option will open up the 'Edit scenario' modal.

<figure><img src="../../.gitbook/assets/scenario-settings.png" alt=""><figcaption><p>Scenario settings option</p></figcaption></figure>

In this modal, you can configure the general and permission settings.

<figure><img src="../../.gitbook/assets/edit-scenario.png" alt=""><figcaption><p>Edit scenario modal</p></figcaption></figure>

If you want to lock your scenario, enable the 'Lock scenario' checkbox. A locked scenario cannot be edited.

<figure><img src="../../.gitbook/assets/lock-scenario.png" alt=""><figcaption><p>Lock scenario option</p></figcaption></figure>

### iii) Input method&#x20;

Inforiver offers two types of input methods, simulation, and distribution.

<figure><img src="../../.gitbook/assets/input-method.png" alt=""><figcaption><p>Input method option</p></figcaption></figure>

#### i) Simulation

If you choose the simulation input method, every data will have the [simulation slider](../4.-adding-business-logic-and-formulae/what-if-analysis-and-simulations.md#ii-simulation-slider), in which you can vary the value to simulate the changes. Once simulations is performed, you can track them below the toolbar.

<figure><img src="../../.gitbook/assets/simulation-method.png" alt=""><figcaption><p>Simulation option</p></figcaption></figure>

#### ii) Distribution

Using this method you can [distribute](../4.-adding-business-logic-and-formulae/budgeting-and-allocations.md) the value across descendants.

<figure><img src="../../.gitbook/assets/distribution-method.png" alt=""><figcaption><p>Distribution option</p></figcaption></figure>

### iii) Show variance

If you enable this option, you will see the percentage of variance to the left of the data metrics.

<figure><img src="../../.gitbook/assets/show-variance.png" alt=""><figcaption><p>Show variance option</p></figcaption></figure>

### iv) Slider settings

If you click the 'Slider settings' option, the 'Variance settings' modal will open up.

<figure><img src="../../.gitbook/assets/variance-settings.png" alt=""><figcaption><p>Variance settings modal</p></figcaption></figure>

This modal has the following options:

i) **Series** - Displays the name of the series in the scenario

ii) **Increase is good** - This toggle is enabled by default. If this is turned on, then the percentage increase will be displayed in green. If this option is disabled, then the increase in value or percentage will be displayed in red.

<figure><img src="../../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>

iii) **Value range** - In this field, you can configure the maximum value of the range. The default is 100%.

In the next section, you will learn about [budgeting and allocations](../4.-adding-business-logic-and-formulae/budgeting-and-allocations.md).
