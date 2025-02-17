# Create new subscription

With Inforiver, creating report subscriptions is easier than ever. Inforiver offers plenty of configurations to create and schedule your subscriptions.

You have the option of starting a **standard subscription** or a **dynamic subscription**.

[Standard Subscription:](./#id-1.-standard-subscription) A standard subscription sends the report to specific recipients configured in the subscriptions page based on the filters and bookmarks if any. The intended recipients for each category/dimension can be manually configured using filters, or can be uploaded in bulk via a CSV file that contains the recipients with filter details.

[Dynamic Subscription:](./#id-2.-dynamic-subscription) A dynamic subscription is similar to the standard subscription, but instead of configuring the report filters manually for each user email ID, we let Inforiver implicitly regulate the dimension categories and share the relevant data with the intended recipient mentioned in the report dataset. With dynamic subscription, you can automatically tailor your report deliveries based on the recipients while also including other dimension filters in the setup.

## 1. Standard Subscription

{% hint style="info" %}
By default, when you start a new subscription, you are initiating a standard subscription.
{% endhint %}

To create a new schedule from the report, publish the report to the Power BI service and click on the **New Subscription** option in the **Export** tab.

<figure><img src="../../../.gitbook/assets/image (885).png" alt=""><figcaption><p>New Subscription from report</p></figcaption></figure>

Alternatively, you can start a new subscription by clicking **New Subscription -> Standard Subscription** (or just the **New Subscription** button) on the **My Subscriptions** page in the Inforiver console.

<figure><img src="../../../.gitbook/assets/image (886).png" alt=""><figcaption><p>New subscription from Inforiver console</p></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (888).png" alt=""><figcaption><p>Starting a new subscription (standard)</p></figcaption></figure>

## 2. Dynamic Subscription

{% hint style="info" %}
This feature is useful for reports or datasets that already include the recipients' Email IDs based on the category/division.&#x20;

You can also get the recipients' email addresses from other semantic models or by importing a CSV file that includes them.
{% endhint %}

With dynamic subscriptions, Inforiver can detect email IDs from your semantic models/CSV files and automatically customize the report based on the user. You can also specify dimension filters to send only specific categories to the users.

To start a dynamic subscription, click **New Subscription -> Dynamic Subscription** from the **My Subscriptions** page in the console.

<figure><img src="../../../.gitbook/assets/image (889).png" alt=""><figcaption><p>Starting a dynamic subscription</p></figcaption></figure>

## 3. Subscription page settings

Starting a new subscription (standard or dynamic) takes you to the 'New subscription' page of the Inforiver Scheduler application. It has 3 tabs: 'Select Report', 'Set Subscription Frequency', and 'Select Destinations' where you can configure all your subscription settings.

{% hint style="info" %}
**For dynamic subscription, you can configure the table selection in the third tab: 'Select Destinations'. All other settings are the same as that of a standard subscription.**
{% endhint %}

Click on the 'Pencil' icon on the top of the 'New subscription' page to edit the name of the subscription.

<figure><img src="../../../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Inforiver subscription name</p></figcaption></figure>

In the upcoming pages, we will discuss the tabs in detail.

**1.** [**Select a report:**](select-a-report.md) You can select your workspace, report, and configure other report-related details in this section.&#x20;

**2.** [**Set subscription frequency:**](set-subscription-frequency.md) Here, you can set the subscription frequency, time, and the start and end dates.&#x20;

**3.** [**Select destinations:**](select-destination-s/) Select where you want your scheduled report to be delivered in the preferred formats (Excel/PDF/PPT), along with the report link and preview.

**4.** [**Review & save subscription:**](review-and-save-subscription.md) You can review your subscription details here and then save or edit the subscription.&#x20;
