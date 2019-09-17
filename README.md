
# serverless-nodejs-aws-demo

## Getting Started 

### What is serverless framework??


### Serverless framework application model:

- Functions: which executes some code in response to some events.

- Events: Like HttpRequest, a schedule timer event or infrastructure provider event like aws s3 fileupload event

        In AWS, you can trigger functions with the events from API Gateway, s3, CloudWatch, DynamoDb

- Resources: Infrastructure that your application depends on ex: dynamodb table, aws s3 bucket etc.

- Serverless Services: A service is like a project. It's where you define your AWS Lambda functions, the events that trigger them and any AWS Infrastructure resources they require, all in a file called serverless.yml. 
A fullblown application can have many services.



### Pre-requisites:

- NodeJs
- Serverless Framework CLI
- AWS CLI

```
$node -v

Install serverless framework:
$npm install serverless -g 

$serverless -v  (or) sls -v

$aws --version

```

### 2. Create a sample service (serverless framework service) project from a template

```
serverless create --template aws-nodejs --path <<servicename>>

serverless deploy
serverless deploy function  --function Emailer
serverless deploy --package package-path
```

### 3. Deploy sample service (serverless framework service) 

```
serverless deploy
(or)
serverless deploy function  --function Emailer
(or)
serverless deploy --package package-path
```

 









