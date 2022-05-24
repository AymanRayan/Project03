# Pipeline

## Dependencies
- github repository
- CircleCI with access to the repository

## Steps started on each push to the repository
- Set up basic functionality
  - Install Node.js
  - Checkout code
  - Install AWS CLI
  - Configure AWS
  - Set up Elastic Beanstalk
- Install backend
- Install frontend
- Build backend
- Build frontend
- Deploy backend (in Elastic Beanstalk environment)
- Deploy frontend (in S3 bucket)


## Description
The pipeline involves one job and one workflow - I know this needs to be made
more granular in larger projects.
of CircleCI. It uses a docker image with Node.js v16, because the default stable
image seems to be shipping with v17 which caused trouble with some library that
required OpenSSL settings.


## Diagram
![Diagram pipeline](diagrams/pipeline.drawio.png)