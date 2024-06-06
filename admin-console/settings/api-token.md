# API token

We provide an API token management system in the admin console where admins can create and manage API tokens. These tokens can then be integrated into any external application to initiate a subscription job, refresh a semantic data input model, or both. This way, any authorized user can start a subscription job or refresh the semantic model with a simple click of a button from an external application without logging in to the admin console or the report.&#x20;

Let us now see the process of creating an API token.

## Create API Token

1. To create a new API token, click **Create API Token** in the API token screen.

<figure><img src="../../.gitbook/assets/image (748).png" alt=""><figcaption><p>Create API token</p></figcaption></figure>

2. In the next screen, you can enter the details of the token.

**Token name:** Enter a name for the token.

**Expiry:** Set the token's validity to 30/60/90 days, or you can set any custom date within a year.

**Description:** Enter an optional description of the token.

**Permission:** You can set either or both of the following permissions: execute a new subscription, and refresh a semantic data input model.

After entering the details, click **Generate**.

<figure><img src="../../.gitbook/assets/image (749).png" alt=""><figcaption><p>Generate token</p></figcaption></figure>

3. A new token will be generated. Ensure it is copied, as it becomes irretrievable after closing the window.

<figure><img src="../../.gitbook/assets/image (750).png" alt=""><figcaption><p>Copy the token</p></figcaption></figure>

Now with this token, we can initiate a scheduled subscription and refresh the semantic data input model externally from any application.

## **Trigger subscriptions from external applications**

By integrating the [created API token](api-token.md#create-api-token) into the required application, you can create an API that triggers the required subscription job. Let us now demonstrate this with the help of the Postman application.

1. You can choose the required subscription from the subscription list or [create a new one.](../../working-with-inforiver/11.-scheduling-reports/create-new-subscription/) Let us run the subscription shown below using the API token.

<figure><img src="../../.gitbook/assets/image (751).png" alt=""><figcaption><p>Scheduled Subscription</p></figcaption></figure>

2. We will now trigger the subscription job using Postman.

<figure><img src="../../.gitbook/assets/image (752).png" alt=""><figcaption><p>Subscription details</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/9.1.2..png" alt=""><figcaption><p>Subscription job triggered</p></figcaption></figure>

3. The report is delivered to the intended recipients as scheduled.

<figure><img src="../../.gitbook/assets/image (754).png" alt=""><figcaption><p>Report delivered</p></figcaption></figure>

## **Refresh semantic data input source using API**

You can also generate API tokens to sync the semantic data input model included in your report to make the latest data available.

1. In the API token management screen, check the ‘Refresh Semantic Data Input’ option and generate the token.

<figure><img src="../../.gitbook/assets/9.2.1. sync refresh data input model-1.png" alt=""><figcaption><p>Refresh Semantic Data Input</p></figcaption></figure>

2. This token can create an API that refreshes the semantic data input source used in your report. The following sample report has a [single-select data input column](../../working-with-inforiver/4.-adding-business-logic-and-formulae/insert-manual-input-columns/dropdown/#id-1.-creating-a-list-of-values) and uses a semantic data input model. Instead of a scheduled refresh, the semantic model is set to be refreshed manually by the user when required.

<figure><img src="../../.gitbook/assets/9.2.2. report with semantic model.png" alt=""><figcaption><p>Report with a semantic data input model</p></figcaption></figure>

3. We will now trigger the synchronization of the semantic data input model, as demonstrated below using Postman.

<figure><img src="../../.gitbook/assets/9.2.3. sync refresh data input model-1.1.png" alt=""><figcaption><p>successfully triggered the refresh of semantic data input</p></figcaption></figure>

4. The data is refreshed, which can be verified from the updated report.

<figure><img src="../../.gitbook/assets/9.2.4. sync refresh data input model-2.png" alt=""><figcaption><p>Updated report</p></figcaption></figure>
