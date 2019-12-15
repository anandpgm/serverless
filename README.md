follow the steps below to create and deploy your first serverless microservice in minutes.

    Install via npm:

npm install -g serverless

    Set-up your Provider Credentials. Watch the video on setting up credentials

    Create a Service:

You can create a new service or install existing services.

# Create a new Serverless Service/Project
serverless create --template aws-nodejs --path my-service
# Change into the newly created directory
cd my-service

    Deploy a Service:

Use this when you have made changes to your Functions, Events or Resources in serverless.yml or you simply want to deploy all changes within your Service at the same time.

serverless deploy -v

    Deploy the Function:

Use this to quickly upload and overwrite your AWS Lambda code on AWS, allowing you to develop faster.

serverless deploy function -f hello

    Invoke the Function on AWS:

Invokes an AWS Lambda Function on AWS and returns logs.

serverless invoke -f hello -l

    Invoke the Function on your machine:

Invokes an AWS Lambda Function on your local machine and returns logs.

serverless invoke local -f hello -l

    Fetch the Function Logs:

Open up a separate tab in your console and stream all logs for a specific Function using this command.

serverless logs -f hello -t

    Remove the Service:

Removes all Functions, Events and Resources from your AWS account.

serverless remove

How to Install a Service:

This is a convenience method to install a pre-made Serverless Service locally by downloading the Github repo and unzipping it. Services are listed below.

serverless install -u https://github.com/your-url-to-the-serverless-service