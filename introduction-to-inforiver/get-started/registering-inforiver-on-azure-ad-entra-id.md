# Registering Inforiver on Azure AD (Entra ID)

Azure active directory app registration is required for every app that requires Microsoft to perform Identity and Access Management. Additionally, Inforiver uses multiple Office 365 APIs to fetch information like Power BI report metadata, user emails and groups, SharePoint, and OneDrive integration, etc. This requires app registration to deploy Inforiver successfully.

## Pre-requisite

We will use certificate-based authentication for Microsoft Entra ID. Follow the steps outlined in the Microsoft documentation to create a self-signed public certificate.

{% embed url="https://learn.microsoft.com/en-us/entra/identity-platform/howto-create-self-signed-certificate" %}
Steps to create a self-signed certificate
{% endembed %}

## Registering the Inforiver application

**STEP 1:** Login into your Azure Portal.

**STEP 2:** Click on **Manage Azure Active Directory** from the menu.

**STEP 3:** Click **App registrations** from the left sub-menu.

**STEP 4:** Click the **New Registration** tab in the top menu bar as shown.

<figure><img src="../../.gitbook/assets/image (1).png" alt=""><figcaption><p>Click the New registration tab</p></figcaption></figure>

**STEP 5:** Enter an **Application Name** to be displayed to the users&#x20;

**STEP 6:** Select **Accounts in this organizational directory only** for the **Who can use this application** option.

**STEP 7:** Leave the **Redirect URI** blank for now. This needs to be filled in after we get the application URL.

**STEP 8:** Click Register to register the application.

<figure><img src="../../.gitbook/assets/image (1) (2).png" alt=""><figcaption><p>Enter details to register the app</p></figcaption></figure>

## Uploading your self-signed certificate

**STEP 1:** Click on **Certificates & secrets** in the left-hand menu.

**STEP 2:** Navigate to Certificates > Upload certificate.

**STEP 3:** Select the certificate file to upload. It must be one of the following file types: .cer, .pem, .crt.&#x20;

**STEP 4:** Click Add.

<figure><img src="../../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

## Environment variable settings

Navigate to your app service and select Environment variables from the left-hand side menu.

Add the variables listed below:

* **O365\_APP\_CERTIFICATE\_CREDENTIALS**: Self-signed certificate body.

<figure><img src="../../.gitbook/assets/image (5).png" alt=""><figcaption><p>Environment variable for Certificate body</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (6).png" alt=""><figcaption><p>End of Certificate body</p></figcaption></figure>

* **O365\_APP\_PRIVATE\_KEY:** Self-signed certificate private key.

<figure><img src="../../.gitbook/assets/image (8).png" alt=""><figcaption><p>Environment variable for RSA private key</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (9).png" alt=""><figcaption><p>End of private key</p></figcaption></figure>

* **O365\_APP\_CERTIFICATE\_THUMBPRINT: T**humbprint value of self-signed certificate. This can be obtained from your Azure AD application Certificate section.

<figure><img src="../../.gitbook/assets/image (3).png" alt=""><figcaption><p>Add environment variables</p></figcaption></figure>

Save the settings after all three environment variables are added. The appservice will restart automatically to reflect the changes.

