# Central Cypress CI/CD Configuration

## About the Project

This project provides a centralized, reusable GitLab CI/CD configuration for Cypress projects. It aims to simplify and standardize the setup and maintenance of Continuous Integration and Continuous Deployment across multiple Cypress-based projects.

### Key Features

- **Centralized Management**: A single CI/CD configuration for all Cypress projects.
- **Efficiency**: Reduces redundancies and simplifies updates across projects.
- **Flexibility**: Easily integrable into new and existing projects.

## Setup and Usage

### Prerequisites

- GitLab account and basic understanding of GitLab CI/CD.
- Projects that use Cypress for end-to-end testing.

### Integrating into Your Project

1. **Include the Central Configuration**:
   In the `.gitlab-ci.yml` file of your Cypress project, add the following `include` statement:

   ```yaml
   include:
     - project: 'namespace/central-repo'
       file: 'central-cypress-ci.yml'
       ref: 'main'

