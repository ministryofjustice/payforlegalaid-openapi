# PayForLegalAid-OpenApi

[![Ministry of Justice Repository Compliance Badge](https://github-community.service.justice.gov.uk/repository-standards/api/payforlegalaid-openapi/badge)](https://github-community.service.justice.gov.uk/repository-standards/payforlegalaid-openapi)

This repository provides the openapi files for use by other payforlegalaid projects.

## Included Files

The repository includes:

- swagger.yaml

## How to use this repository
TBD - awaiting hosting implementation

## Versioning
On creation of a pull request, the `increment version` workflow will run, and automatically increment the patch version number by one. 
Commits are signed using an SSH key. The private key is stored as a secret in GitHub and should be maintained by a current member of the team.

This is to support correct values for package deployment and tag creation.

## How to deploy a new version of payforlegalaid-openapi
* Raise PR for review, requires two approvals
* Merge change into main - this will trigger the package deployment workflow
* Review of workflow will be required, request from member of the GPFD team

## Tags
On deployment of a new package, the CI/CD pipeline will also tag the software 

Tagging follows the naming convention vX.X.X, where X.X.X is the version defined in the `pom.xml`. If tag name pattern is altered in workflow, and does not follow convention, the tag creation will fail.

## Pre commit hooks
Pre commit hooks have been set up on this repository to ensure no accidental commits of secrets, keys etc. Provided by DevSecOps https://github.com/ministryofjustice/devsecops-hooks