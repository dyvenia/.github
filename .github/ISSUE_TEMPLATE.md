name: Deployment
description: Deployment issue template
title: "[Deployment]: "
labels: ["deployment", "triage"]
assignees:
  - devops
body:
  - type: dropdown
    id: environment
    attributes:
      label: Environment
      description: Specify the deployment environment
      options:
        - Development
        - Test
        - Production
    validations:
      required: true
  - type: input
    id: project-name
    attributes:
      label: Project Name
      description: Specify the name of the project
      placeholder: Enter the project name
    validations:
      required: true
  - type: markdown
    attributes:
      value: |
        Thanks for taking the time to fill out this deployment request!
  - type: input
    id: contact
    attributes:
      label: Contact Details
      description: How can we get in touch with you if we need more info?
      placeholder: ex. John Doe
    validations:
      required: true
  - type: textarea
    id: short-description
    attributes:
      label: Short Description
      description: Provide a concise summary of the deployment
      placeholder: Briefly describe the purpose of this deployment
    validations:
      required: true
  - type: dropdown
    id: change-type
    attributes:
      label: Change Type
      description: Specify the type of change being made
      options:
        - Hotfix
        - New Feature
        - Refactoring
    validations:
      required: true
  - type: input
    id: deployment-time
    attributes:
      label: Preferred Deployment Time and Date
      description: Indicate the desired time and date for the deployment
    validations:
      required: true
  - type: textarea
    id: impact
    attributes:
      label: Impact
      description: Describe the anticipated impact of the deployment
      placeholder: Explain the expected consequences of this deployment
    validations:
      required: true
  - type: textarea
    id: rollback-plan
    attributes:
      label: Rollback Plan
      description: Outline a plan for reverting the deployment in case of any issues or failures
      placeholder: Describe the steps to revert the deployment if needed
    validations:
      required: false
  - type: textarea
    id: communication-plan
    attributes:
      label: Communication Plan
      description: Define how the deployment will be communicated to stakeholders and team members
      placeholder: Describe the plan for notifying stakeholders and team members
    validations:
      required: false
  - type: checkboxes
    id: change-tested
    attributes:
      label: Change Tested
      description: Has the change been thoroughly tested?
      options:
        - label: "locally"
        - label: "In Development environment"
        - label: "In Test environment"
        - label: "Has not been tested"