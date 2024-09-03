# Admin consent for Inforiver's entra ID

Inforiver is an add-on visual that operates atop the Power BI framework. Power BI does not share user details, hence users must login with their Microsoft O365 account. [Admin consent](admin-consent-for-inforivers-entra-id.md) will be required to login, add writeback destinations, or connect to integrations like Teams or SharePoint.

Users may get an approval window as shown in the screenshot.

<figure><img src="../../../.gitbook/assets/image (511) (1).png" alt=""><figcaption><p>Admin approval screen</p></figcaption></figure>

A tenant admin can provide access by following the steps outlined below.

**STEP 1:** Navigate to the consent URL. The admin can either use the **Copy Link** option highlighted in the screenshot below or open the consent URL:

{% embed url="https://login.microsoftonline.com/organizations/adminConsent?client_id=91891913-3884-46d3-bb4c-f68d33f43d4b&redirect_uri=https://addons.inforiver.com" %}

<figure><img src="../../../.gitbook/assets/image (513) (1).png" alt=""><figcaption><p>Copy the consent URL and open the link</p></figcaption></figure>

**STEP 2:** Approve the requested permissions by clicking on the accept button.

<figure><img src="../../../.gitbook/assets/image (514) (1).png" alt=""><figcaption><p>Click the accept button to approve</p></figcaption></figure>

The user will be able to login to the Inforiver console, connect to integrations, or add writeback destinations once the admin has approved.
