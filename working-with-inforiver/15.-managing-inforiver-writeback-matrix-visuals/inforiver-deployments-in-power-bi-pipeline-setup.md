---
description: Inforiver deployments using Power BI deployment pipelines
---

# Inforiver deployments in Power BI pipeline setup

Let's explore how Inforiver visuals can be deployed using PowerBI deployment pipelines.

**Overview**

PowerBI Deployment pipelines enable creators to develop and test Power BI content in the Power BI service before the content is made available for consumption by users. The tool is designed as a pipeline with multiple stages, for example, development, test, QA, and production. [Read more on PowerBI Deployment Pipelines](https://nam12.safelinks.protection.outlook.com/?url=https%3A%2F%2Flearn.microsoft.com%2Fen-us%2Ffabric%2Fcicd%2Fdeployment-pipelines%2Fintro-to-deployment-pipelines\&data=05%7C01%7CDeepthyD%40lumel.com%7Ca87a79fb0b12450c528508dbc0b0a156%7C9f84ee4bbee342f7b84ce57e5e92f105%7C0%7C0%7C638315637090593779%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000%7C%7C%7C\&sdata=tVBVdrJJ4Zlr4nx%2FV%2FFPPTwvnSB48LD%2BroaOexysB7k%3D\&reserved=0).&#x20;

You can follow the steps outlined in **section 1 to** [**deploy Inforiver visuals with Power BI deployment pipelines**.](inforiver-deployments-in-power-bi-pipeline-setup.md#1.-setup-inforiver-with-powerbi-deployment-pipelines)

Each time you deploy a report from a lower environment to a higher environment (E.g., development to test), the Inforiver visual ID that is assigned to the visual in the lower environment gets assigned to the higher environment. As a result, the enterprise data and settings such as custom columns, comments, and writeback configurations from lower stages get mapped to the visual in the higher stage.

To prevent consumers from using the visual with the lower environment’s visual ID, we need to follow additional steps to [**detach the visual**](inforiver-deployments-in-power-bi-pipeline-setup.md#2.-detach-the-visual) and for [**pipeline recovery**](inforiver-deployments-in-power-bi-pipeline-setup.md#3.-pipeline-recovery-config) which are outlined in **sections 2 and 3.**&#x20;

## 1. Setup Inforiver with PowerBI deployment pipelines

1. Assign workspaces to each stage i.e. the Development/Test/Production stages of the deployment pipeline. [Learn more about assigning workspaces](https://learn.microsoft.com/en-us/fabric/cicd/deployment-pipelines/assign-pipeline).&#x20;

<figure><img src="../../.gitbook/assets/image (10) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Assign workspaces</p></figcaption></figure>

2. Create a report that uses Inforiver visuals. Publish it to the workspace mapped to the first(development) stage of the pipeline. For this demonstration, we have created a report titled 'PD\_Dec19\_2023' under the 'Inforiver - Pipeline - Dev' workspace.&#x20;
3. Navigate to the Deployment Pipelines tab, and select the required pipeline. Select the report to be deployed to the test environment. [Learn more about deploying reports.](https://learn.microsoft.com/en-us/fabric/cicd/deployment-pipelines/deploy-content)

<figure><img src="../../.gitbook/assets/image (333) (1).png" alt=""><figcaption><p>Select items for deployment</p></figcaption></figure>

2. Review the items that are being deployed and click on the Deploy button.

<figure><img src="../../.gitbook/assets/image (334) (1).png" alt=""><figcaption><p>Start deployment</p></figcaption></figure>

2. After the deployment is complete, you will be able to see the report in the next stage, in this case, the Inforiver - Pipeline - Test workspace.

## 2. Detach the visual

When a visual is deployed for the first time in an environment, we need to follow the steps outlined to create a new visual ID. Please note that these steps need to be done only when the visual is deployed for the first time.&#x20;

1. After the deployment is complete, open the report from the target environment, in this case, the Inforiver - Pipeline - Test workspace. A notification is generated, indicating that the visual is a duplicate.

<figure><img src="../../.gitbook/assets/image (337) (1).png" alt=""><figcaption></figcaption></figure>

2. Switch to edit mode and sign in. After signing in, there will be a yellow icon on the top right indicating that the report is a duplicate of the report in the development environment.

<figure><img src="../../.gitbook/assets/image (338) (1).png" alt=""><figcaption></figcaption></figure>

3. Click on _Report Details_ under the user profile. This will open the report details pane.

<figure><img src="../../.gitbook/assets/image (339) (1).png" alt=""><figcaption></figcaption></figure>

4. Click on the Create button to detach this visual and create a new visual ID. A dialog box will pop up.&#x20;

<figure><img src="../../.gitbook/assets/image (340) (1).png" alt=""><figcaption></figcaption></figure>

5. The dialog box gives two options to populate data input values in the visual:

* To copy values from the lower environment to the higher environment, select the "Yes, I do" option.
* To fill in new values, select the "No, I will start with blank cell values" option.

Tick the confirmation checkbox and click on the Proceed button to save the report.

<figure><img src="../../.gitbook/assets/image (341) (1).png" alt=""><figcaption></figcaption></figure>

6. Save the visual to commit the changes.

<figure><img src="../../.gitbook/assets/image (342) (1).png" alt=""><figcaption></figcaption></figure>

7. Repeat these steps when deploying a report to an environment for the first time.

## 3. **Pipeline recovery config**

This section outlines the steps to set up a pipeline recovery configuration. This is a one-time setup that is required for Inforiver to detect pipeline deployments. Pipeline recovery must be configured for every report that is deployed.

1. Click on _Pipeline Recovery Config_ from the user profile menu. This will navigate to the configuration URL.

<figure><img src="../../.gitbook/assets/image (343) (1).png" alt=""><figcaption></figcaption></figure>

2\. Click on the Add Pipeline button or link in the pipeline recovery webpage.

<figure><img src="../../.gitbook/assets/image (344) (1).png" alt=""><figcaption></figcaption></figure>

3\. Enter the configuration details:

* Pipeline Name: User-defined name to identify the pipeline recovery config for a particular report.
* Stage: User-defined name to identify the stage in the deployment pipeline. Each stage defined in the recovery config should correspond to a stage in the Power BI deployment pipeline.
* Visual ID: Unique Inforiver visual ID.

4\. Get the visual IDs for the reports in lower and higher environments from the user profile menu.

<figure><img src="../../.gitbook/assets/image (349).png" alt=""><figcaption></figcaption></figure>

5. After completing the configurations, click on Save.&#x20;

<figure><img src="../../.gitbook/assets/image (350).png" alt=""><figcaption></figcaption></figure>

5. In this example, we are deploying from Dev to Test, so we have created two stages. Click on the Add Stage button to configure additional stages like QA and Prod.

## **4. Pipeline deployment recovery workflow**

&#x20;After deploying a report, when you open the report in a higher environment, you will see a popup saying "Pipeline Deployment Detected".  Please note that Inforiver will detect deployments only if the visual has been detached(step 2) and pipeline recovery(step 3) has been configured.

<figure><img src="../../.gitbook/assets/image (348).png" alt=""><figcaption></figcaption></figure>

Open the report in edit mode to complete pipeline recovery. You will see a notification for successful pipeline recovery after switching to edit mode.

## Writeback Configuration with Pipeline Recover

* When a report is deployed to a higher environment for the first time, on recovery, the writeback settings are not passed on from the lower to the higher environment. The user is expected to configure separate writeback destinations for the higher stage. This is a one-time setup after the initial deployment of the report.
* Once the configuration is done, it is recovered through the pipeline recovery workflow after each deployment.

## Data Input with Pipeline Deployment

* After Pipeline deployment, upon recovery, the data input columns in the visuals in both the lower and the higher environments are compared. The visual in the higher environment is then synced with its lower environment counterpart by the creation/renaming/deletion of the data inputs that are not identical.
* Please note that if a data input field is renamed, the values are retained as is - values in the higher environment will not be overwritten. For Date input columns, the values are also updated.
