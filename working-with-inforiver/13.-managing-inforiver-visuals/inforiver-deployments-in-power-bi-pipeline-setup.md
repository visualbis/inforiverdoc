---
description: Inforiver deployments using Power BI deployment pipelines
---

# Inforiver deployments in Power BI pipeline setup

In this section, let's explore how Inforiver visuals can be deployed using PowerBI deployment pipelines.

PowerBI Deployment pipelines enable creators to develop and test Power BI content in the Power BI service before the content is made available for consumption by users. The tool is designed as a pipeline with three stages: development, test, and production. [Read more on PowerBI Deployment Pipelines](https://nam12.safelinks.protection.outlook.com/?url=https%3A%2F%2Flearn.microsoft.com%2Fen-us%2Ffabric%2Fcicd%2Fdeployment-pipelines%2Fintro-to-deployment-pipelines\&data=05%7C01%7CDeepthyD%40lumel.com%7Ca87a79fb0b12450c528508dbc0b0a156%7C9f84ee4bbee342f7b84ce57e5e92f105%7C0%7C0%7C638315637090593779%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000%7C%7C%7C\&sdata=tVBVdrJJ4Zlr4nx%2FV%2FFPPTwvnSB48LD%2BroaOexysB7k%3D\&reserved=0).&#x20;

## Setup Inforiver with PowerBI deployment pipelines

1. Assign workspaces to the Development/Test/Production stages of the deployment pipeline. [Learn more about assigning workspaces](https://learn.microsoft.com/en-us/fabric/cicd/deployment-pipelines/assign-pipeline).&#x20;

<figure><img src="../../.gitbook/assets/image (10) (1) (1) (1).png" alt=""><figcaption><p>Assign workspaces</p></figcaption></figure>

2. Create a report that uses Inforiver visuals. Publish it to the workspace mapped to the Development Stage of the pipeline. For this demonstration, we have created a report titled 'PipelineDeploy\_Sep28' under the 'Inforiver - Pipeline - Dev' workspace. Select the report to be deployed to the test environment. [Learn more about deploying reports.](https://learn.microsoft.com/en-us/fabric/cicd/deployment-pipelines/deploy-content)

<figure><img src="../../.gitbook/assets/image (11) (1) (1).png" alt=""><figcaption><p>Select items for deployment</p></figcaption></figure>

3. Review the items that are being deployed and click on the Deploy button.

<figure><img src="../../.gitbook/assets/image (12) (1) (1).png" alt=""><figcaption><p>Start deployment</p></figcaption></figure>

4. After the deployment is complete, open the report from the Test environment. A notification is generated, prompting the user to open the report in edit mode.&#x20;
5. After opening the report in edit mode, there will be a yellow icon on the top right indicating that the report is a duplicate of the report in the development environment.

<figure><img src="../../.gitbook/assets/image (13) (1) (1).png" alt=""><figcaption><p>Indicator that report is a duplicate from dev region</p></figcaption></figure>

6. Click on _Report Details_ under the user profile. This will open the report details pane.

<figure><img src="../../.gitbook/assets/image (14) (1) (1).png" alt=""><figcaption></figcaption></figure>

7. Click on the Create button to detach this visual.

<figure><img src="../../.gitbook/assets/image (15) (1) (1).png" alt=""><figcaption></figcaption></figure>

8. Click on the Proceed button to save the report.

<figure><img src="../../.gitbook/assets/image (16) (1) (1).png" alt=""><figcaption></figcaption></figure>

9. Repeat the above steps between the test and production stages to deploy the report to the production environment.

## **Pipeline deployment recovery workflow**

Each time you deploy a report from a lower environment to a higher environment (E.g., development to test), the Inforiver visual ID that is assigned to the visual in the lower environment gets assigned to the higher environment. As a result, the enterprise data and settings such as custom columns, comments, and writeback configurations from lower stages get mapped to the visual in the higher stage.

To prevent the user from using the visual with the lower environment’s visual ID, a blocker screen is displayed, prompting the user to open the report in edit mode. To recover the visual ID of the higher environment, follow the steps listed below after each deployment:

* Open the higher environment report in edit mode.
* Login to the visual and save the report.

## Writeback Configuration with Pipeline Recovery Workflow

* When a report is deployed to a higher environment for the first time, on recovery, the writeback settings are not passed on from the lower to the higher environment. The user is expected to configure separate writeback destinations for the higher stage. This is a one-time setup after the initial deployment of the report.
* Once the configuration is done, it is recovered through the pipeline recovery workflow after each deployment.

## Data Input with Pipeline Deployment

* After Pipeline deployment, upon recovery, the data input columns in the visuals in both the lower and the higher environments are compared. The visual in the higher environment is then synced with its lower environment counterpart by the creation/renaming/deletion of the data inputs that are not identical.
* Please note that if a data input field is renamed, the values are retained as is. For Date input columns, the values are also updated.
