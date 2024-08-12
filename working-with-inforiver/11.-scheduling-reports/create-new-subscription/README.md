# Create new subscription

With Inforiver, creating report subscriptions is easier than ever. Inforiver offers plenty of configurations to create and schedule your subscriptions.

You have the option of starting a **standard subscription** or a **dynamic subscription**.

[Standard Subscription:](./#id-1.-standard-subscription) A standard subscription sends the report to specific recipients configured in the subscriptions page based on the filters and bookmarks if any. The intended recipients for each category/dimension can be manually configured using filters, or can be uploaded in bulk via a CSV file that contains the recipients with filter details.

[Dynamic Subscription:](./#id-2.-dynamic-subscription) A dynamic subscription is similar to the standard subscription, but instead of configuring the report filters manually as per the user email IDs, we let Inforiver to implicitly regulate the dimension categories and share them with the intended report users mentioned in the report dataset.&#x20;

## 1. Standard Subscription

{% hint style="info" %}
By default, when you start a new subscription, you are initiating a standard subscription.
{% endhint %}

To create a new schedule from the report, publish the report to the Power BI service and click on the **New Subscription** option in the **Export** tab.

<figure><img src="../../../.gitbook/assets/image (885).png" alt=""><figcaption><p>New Subscription from report</p></figcaption></figure>

Alternatively, you can start a standard subscription by clicking **New Subscription -> Standard Subscription** (or just the **New Subscription** button) on the **My Subscriptions** page in the admin console.

<figure><img src="../../../.gitbook/assets/image (886).png" alt=""><figcaption><p>New subscription from admin console</p></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (888).png" alt=""><figcaption><p>Starting a standard subscription</p></figcaption></figure>

## 2. Dynamic Subscription

{% hint style="info" %}
This feature can be used for reports or datasets that already contain Email IDs.
{% endhint %}

With dynamic subscriptions, Inforiver can detect email IDs from your semantic models/CSV files and automatically send the report to a specific user. You can also specify dimension filters to send only those categories to the users.

If your report contains user email IDs and you wish to start a dynamic subscription, click **New Subscription -> Dynamic Subscription** from **My Subscriptions** page in the admin console.

<figure><img src="../../../.gitbook/assets/image (889).png" alt=""><figcaption><p>Starting a dynamic subscription</p></figcaption></figure>

## 3. Subscription page settings

Starting a new subscription (standard or dynamic) takes you to the 'New subscription' page of the Inforiver Scheduler application. It has 3 tabs: 'Select Report', 'Set Subscription Frequency', and 'Select Destinations' where you can configure all your subscription settings.

{% hint style="info" %}
For dynamic subscription, you can configure the table selection in the third tab: 'Select Destinations'. All other settings are the same as that of a standard subscription.
{% endhint %}

Click on the 'Pencil' icon on the top of the 'New subscription' page to edit the name of the subscription.

<figure><img src="../../../.gitbook/assets/image (887).png" alt=""><figcaption><p>Inforiver subscription name</p></figcaption></figure>

In the upcoming pages, we will discuss the tabs in detail.

**1. Select a report** - You can select your workspace, report and configure other report-related details. To learn more, refer to [select a report](select-a-report.md).

**2. Set subscription frequency** - You can configure and set the subscription frequency. To learn more, refer to [set subscription frequency](set-subscription-frequency.md).

**3. Select destinations** - You can select the destinations to schedule your subscriptions. To learn more, refer to [select destinations](select-destination-s/).

**4. Review & save subscription** - You can easily review your subscription details, save or edit the subscription. To learn more, refer to [review & save subscription](review-and-save-subscription.md).
