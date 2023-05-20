# Deployment Request Repository

This repository is used for creating deployment requests for the DevOps team. It provides a structured GitHub issue template that gathers all the necessary information for initiating a deployment. The template ensures that all required details are provided, facilitating the deployment process.

## How to Create a Deployment Request

1. Click on the **Issues** tab at the top of the repository.
2. Click the green **New Issue** button.
3. Select the **Deployment** issue template from the available templates.
4. Fill out the requested information in the form.
5. Provide a concise summary of the deployment in the **Short Description** section.
6. Select the appropriate environment from the **Environment** dropdown.
7. Specify the name of the project in the **Project Name** field.
8. Enter your contact details, so the DevOps team can reach out to you if needed.
9. Choose the type of change being made from the **Change Type** dropdown.
10. Indicate the preferred deployment time and date.
11. Describe the anticipated impact of the deployment in the **Impact** section.
12. (Optional) Outline a rollback plan in the **Rollback Plan** section.
13. (Optional) Define the communication plan for notifying stakeholders and team members in the **Communication Plan** section.
14. Select the appropriate option regarding the testing of the change from the **Change Tested** checkboxes.
15. Click the green **Submit New Issue** button to create the deployment request.

## Repository Structure

- `deployment.yaml`: This file defines the GitHub issue template for deployment requests. It contains fields for capturing relevant information such as environment, project name, contact details, change type, deployment time, impact, rollback plan, communication plan, and change testing.

## Discussion

Feel free to discuss any deployment requests or related topics in the [#devops](https://dyveniaworkspace.slack.com/archives/C042PFLG62K) channel on Slack. This channel is dedicated to discussing deployments, infrastructure, and other DevOps-related matters.