# Email Campaign

![node.js](https://img.shields.io/badge/Node%20JS-12-green?style=for-the-badge&logo=appveyor)


## Description
**API REST** for Send RAW Email in a massive quantity (request an Increase of Quota Limit if your **AWS SES** have a short amount of messages for the requirements).



## Description of the API
Internally use a AWS Pipeline to determine Bounces and Complaints.

Following some these tutorials and pipelines from AWS Knowledge Center:

- [AWS Lambda Function for SES to DynamoDB](https://aws.amazon.com/premiumsupport/knowledge-center/lambda-sns-ses-dynamodb/)

- [Maintaining a Healthy Email Database with AWS Lambda, Amazon SNS, and Amazon DynamoDB](https://aws.amazon.com/blogs/compute/maintaining-a-healthy-email-database-with-aws-lambda-amazon-sns-and-amazon-dynamodb/)


## Pipeline
[![Pipeline](https://awscomputeblogimages.s3-us-west-2.amazonaws.com/healthy_Picture1.png)](https://aws.amazon.com/blogs/compute/maintaining-a-healthy-email-database-with-aws-lambda-amazon-sns-and-amazon-dynamodb/)


## Routes
- **[GET] /**: Returrn to the client a tiny welcome object. (JSON Format).
- **[POST] /send/email**: Start the massive send of emails. Follow the Postman Collection 



## Notes

 - This project have not Unit Testings so, do not expect it.

 - You need to have your own AWS Set of Services working propperly.

 - Probabbly in the future, API REST can have errors handlers to inform the client what it is going wrong with the request.

 - Many of the functions have a strongs commentaries for explaining what kind of magic I did.

 - Rename the *test.env* file into *.env*
