# Basic consent

When users login to the Inforiver portal for the first time, admin consent will be required to authenticate the user. The portal utilizes Inforiver’s Entra ID app to authenticate the user and admins need to provide consent for users to be able to login.

**STEP 1:** Admins can directly navigate to the consent URL.&#x20;

```
https://login.microsoftonline.com/common/oauth2/v2.0/authorize?client_id=91891913-3884-46d3-bb4c-f68d33f43d4b&response_type=code&redirect_uri=https%3A%2F%2Faddons.inforiver.com%3A443%2FRedirect&response_mode=form_post&scope=https%3A%2F%2Fgraph.microsoft.com%2FUser.ReadBasic.All https%3A%2F%2Fanalysis.windows.net%2Fpowerbi%2Fapi%2FReport.Read.All https%3A%2F%2Fanalysis.windows.net%2Fpowerbi%2Fapi%2FDataset.Read.All https%3A%2F%2Fanalysis.windows.net%2Fpowerbi%2Fapi%2FWorkspace.Read.All https%3A%2F%2Fgraph.microsoft.com%2FGroup.Read.All https%3A%2F%2Fgraph.microsoft.com%2FGroupMember.Read.All&prompt=consent
```

Users can either use the **Copy Link** option highlighted in the screenshot below or open the consent URL and share it with the admin.

<figure><img src="../../../../.gitbook/assets/image (2) (1).png" alt=""><figcaption><p>Admin approval notification</p></figcaption></figure>

**STEP 2:** Admins can approve the permissions listed in the screenshot to allow users to login.

<figure><img src="../../../../.gitbook/assets/image (3) (1).png" alt=""><figcaption><p>Permissions required for user login</p></figcaption></figure>

**STEP 3:** Additional permissions are required to add functionalities like inviting other users in the organization and connecting to Power BI with Inforiver. Admins can navigate to the consent URL:

```
https://login.microsoftonline.com/common/oauth2/v2.0/authorize?client_id=91891913-3884-46d3-bb4c-f68d33f43d4b&response_type=code&redirect_uri=https%3A%2F%2Faddons.inforiver.com%3A443%2FRedirect&response_mode=form_post&scope=https%3A%2F%2Fgraph.microsoft.com%2FUser.ReadBasic.All https%3A%2F%2Fanalysis.windows.net%2Fpowerbi%2Fapi%2FReport.Read.All https%3A%2F%2Fanalysis.windows.net%2Fpowerbi%2Fapi%2FDataset.Read.All https%3A%2F%2Fanalysis.windows.net%2Fpowerbi%2Fapi%2FWorkspace.Read.All https%3A%2F%2Fgraph.microsoft.com%2FGroup.Read.All https%3A%2F%2Fgraph.microsoft.com%2FGroupMember.Read.All&prompt=consent
```

Admins need to provide all the permissions shown in the screenshot and check the ‘Consent on behalf of your organization’ option.

<figure><img src="../../../../.gitbook/assets/image (4) (1).png" alt=""><figcaption><p>Power BI related permission</p></figcaption></figure>

Note: After clicking  Accept, admins may get a ‘Login Failed’ page, this is expected behavior if they aren’t a member of the Inforiver portal.

**STEP 4:** After providing permissions, the Inforiver Entra ID app’s permissions page in the Enterprise Applications section should look like this.

<figure><img src="../../../../.gitbook/assets/image (1268).png" alt=""><figcaption><p>Inforiver Entra ID app permission page</p></figcaption></figure>
