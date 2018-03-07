Welcome to NimbusWeb
==================================================

This code Node.js web serverless app service deployed by AWS CloudFormation to AWS Lambda and Amazon API Gateway.

What's Here
-----------

This sample includes:

* README.md - this file
* buildspec.yml - this file is used by AWS CodeBuild to package the 
  application for deployment to AWS Lambda
* public/ - directory containing web code copies tp S3 bucket as a part of deployment
* template.yml - this file contains the AWS Serverless Application Model (AWS SAM) used
  by AWS CloudFormation to deploy the application to AWS Lambda and Amazon API
  Gateway.
* tests/ - this directory contains unit tests for the application


How to proceed
------------------

To run your tests locally, go to the root directory of the 
sample code and run the `nom install; npm test` commands, which
AWS CodeBuild also runs through your `buildspec.yml` file.
 
To test the new code during the release process, modify the existing tests or 
add tests to the tests directory. AWS CodeBuild will run the tests during the 
build stage of the project pipeline. You can find the test results
in the AWS CodeBuild console.
 
