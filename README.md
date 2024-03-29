# AWS Wiremock Server

#### Description
This repository is used to manage and maintain a mocking framework hosted in AWS. 

The framework relies on Wiremock docker images hosted in an AWS ECR which are then used with Fargate Services to give the consumer a constant mocked server.

The mocks that the server will provide are defined in the `mappings` and `__files` folders. There are provided examples for each given.

#### To Update Mocks

To update the mocks served by wiremock follow the below steps. 

1. Clone this repository to your local machine
2. Add in a new mappings file to the `mappings` folder. This must be a JSON file and have both a `request` and `response` section. For a more detailed explanation: [Wiremock Stubbing](https://wiremock.org/docs/stubbing/)
3. Once your new mapping has been added, merge your change back into this repository and the server will be updated automatically.

#### TODO:
- Fill our the README with a more detailed explanation 
- Add more resources to the How-To (looking at coniditationl mockings and such)
