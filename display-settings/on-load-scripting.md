# On-load scripting

Inforiver’s on-load scripting feature enables you to list a set of actions to be performed on loading the visual. You can display messages, set the layout, hide columns, or apply filters as the visual is loaded. The scripts will be executed when you open the report, switch to the tab containing the visual, or refresh the visual. &#x20;

Inforiver offers an array of built-in functions that you can use to set up scripts effortlessly. [Learn more about scripting functions.](../formula-syntax/scripting-functions/)

<figure><img src="../.gitbook/assets/1. Onload scripts.png" alt=""><figcaption><p>On load scripts</p></figcaption></figure>

Notice how all the scripts have been executed when the visual is loaded.

{% hint style="info" %}
To see the scripts in action, click the Run now button
{% endhint %}

<figure><img src="../.gitbook/assets/1.1 Onload scripts output.png" alt=""><figcaption><p>Executing on-load scripts</p></figcaption></figure>

Let's look at some applications of on-load scripts.

#### 1. Displaying messages

You can display custom text as a toast message notification. The supported types include alerts, information, warnings, and success messages among others. [Learn more about the DISPLAYTOAST function.](../formula-syntax/scripting-functions/displaytoast.md)

<div>

<figure><img src="../.gitbook/assets/image (704).png" alt=""><figcaption><p>Alert message</p></figcaption></figure>

 

<figure><img src="../.gitbook/assets/info.png" alt=""><figcaption><p>Info message</p></figcaption></figure>

 

<figure><img src="../.gitbook/assets/warning (1).png" alt=""><figcaption><p>Warning message</p></figcaption></figure>

</div>

#### 2. Setting the layout

You can set a particular theme or expand hierarchical data to a specific level. [Learn more about the LAYOUT function](../formula-syntax/scripting-functions/layout.md).

<div>

<figure><img src="../.gitbook/assets/image (705).png" alt=""><figcaption><p>Setting the theme and layout</p></figcaption></figure>

 

<figure><img src="../.gitbook/assets/hierarchy level.png" alt=""><figcaption><p>Navigating to a particular hierarchy level</p></figcaption></figure>

</div>

#### 3. Filtering periodic data

You can filter the data to show only a specific time period, for instance, the last 4 months or the last 2 years. [Learn more about filtering time series data](../formula-syntax/scripting-functions/showbetweenperiod.md).

<figure><img src="../.gitbook/assets/image (706).png" alt=""><figcaption><p>Displaying next 4 months when current month is May</p></figcaption></figure>
