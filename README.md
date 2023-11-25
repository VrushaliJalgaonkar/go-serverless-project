# Go-serverless-project

## Technologies used
Go, version - 1.19  
AWS SDK  
AWS Lambda  
AWS Lambda Events  
AWS Session  
AWS DynamoDB  
AWS DynamoDB Dynamodbiface  
AWS API Gateway


## Project Introduction  
Created a CRUD project using Go along with AWS, to create data, read data, update existing data and delete data from AWS DynamoDB. Also used AWS session, AWS Lambda and AWS Lambda Events to create REST APIs.

## Build project

Install [AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html).  

Install depenedncies:  
``` 
go mod tidy
```   
  
Build the main.go
``` 
go build main.go
``` 
Move main build from main folder to build folder

Create a zip, to deploy on AWS  
``` 
zip -jrm build/main.zip build/main
``` 

Upload zip to AWS serverless, configure AWS DynamoDB and AWS APIGateway.

## AWS DynamoDB information  
Table name = 'go-serverless-project'  
Table structure:  
Column names | Data type :  
``` 
Email     string (Primary Key)   
FirstName string  
LastName  string   
```



