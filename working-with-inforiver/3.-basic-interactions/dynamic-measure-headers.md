# Dynamic measure headers

To change the name of a measure, double-click on the measure header and rename it to a relevant name. Inforiver also offers capabilities to dynamically generate headers, which we will explore in this section.

### i) Use predefined functions

Inforriver's predefined functions can be leveraged to create dynamic headers. To view the list of available functions, double-click the header and press ctrl + space.&#x20;

<figure><img src="../../.gitbook/assets/image (208).png" alt=""><figcaption><p>Predfined functions for headers</p></figcaption></figure>

On selecting the 'Returns the current Month' option, the month name is appended to the measure header.

<figure><img src="../../.gitbook/assets/image (210).png" alt=""><figcaption><p>Month name appended to header</p></figcaption></figure>

#### Using Operators with predefined functions

We can also use operations such as + or - in conjunction with predefined functions. In the example below, we are using the - operator to access the previous month.

<figure><img src="../../.gitbook/assets/image (213).png" alt=""><figcaption><p>Using operators with predefined functions</p></figcaption></figure>

Using the - operator, the previous quarter and previous month have been dynamically appended to the measure headers.

<figure><img src="../../.gitbook/assets/image (215).png" alt=""><figcaption></figcaption></figure>

#### Setting the fiscal period

The accounting period can be defined using the ‘Fiscal year start month’ option in the Misc tab under Display settings. The built-in FISCAL\_QUARTER() function will return the quarter based on the defined start month.&#x20;

<figure><img src="../../.gitbook/assets/image (216).png" alt=""><figcaption><p>Fiscal year start month setting</p></figcaption></figure>

Notice how the fiscal quarter is set to Q2 in the measure header on choosing April as the fiscal year start month.

<figure><img src="../../.gitbook/assets/image (217).png" alt=""><figcaption><p>Fiscal quarter based on fiscal year start settings</p></figcaption></figure>

### ii) Reference grid value

We can also directly reference values from the grid in measure headers. To achieve this, add the field to be referenced as the 'Others' parameter of the visual. Double-click on the header to edit it and select the value to be referenced from the grid. To remove the field from the report, hide the field from 'Manage Columns'.&#x20;

<figure><img src="../../.gitbook/assets/image (218).png" alt=""><figcaption></figcaption></figure>

In the next section, we'll cover some [basic actions](actions/) such as selections and formatting using rails, toolbar customizations, keyboard shortcuts, and reset.
