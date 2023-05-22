name: Deployment
description: Deployment issue template
title: "[Deployment]: "
labels: ["deployment", "triage"]
assignees:
  - devops
body:
  - type: markdown
    attributes:
      value: |
        Thanks for taking the time to fill out this deployment request!
  - type: checkboxes
    id: environment
    attributes:
      label: Environment
      description: Specify the deployment environment
      options:
        - labe: "Development"
        - labe: "Test"
        - labe: "Production"
    validations:
      required: true
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
  - type: textarea
    id: short-description
    attributes:
      label: Short Description
      description: Provide a concise summary of the deployment
      placeholder: Briefly describe the purpose of this deployment
    validations:
      required: false