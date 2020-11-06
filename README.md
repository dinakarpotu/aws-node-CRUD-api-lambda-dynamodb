# aws-node-CRUD-api-lambda-dynamodb
Example sets up AWS serverless backend to create, list, get, update and delete DB records. 
API Gateway acts as REST API, Lambda as functions and DynamoDB to store the data. 
# Structure
Refer to api folder for CRUD services. 
API Gateway -> Lambda -> DynamoDB
API Gateway CORS enabled + Custom domain with API SSL certificate
# Use Cases
API for frontend Web App || 
API for frontend Mobile Ap || 
API for CRUD functionality
# Scaling
API Gateway + Lambda provides auto-scaling. Lambda concurrent executions upto 1000
Increase DynamoDB ProvisionedThroughput: RCU and WCU in serverless.yml
# Serverless Framework
Serverless Framework to deploy the complete stack on fly and remove on fly. Custamize the serverless.yaml template refering to comments in [BOLD].
# CI/CD
Create AWS CodePipeline and use the buildspec.yml template to Automate Code Deployment. Everytime a git commit CodePipeline auto deploys.