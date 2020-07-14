# igniteDelawareIAC-July2020

## Purpose
This Ignite Delaware Infrastructure as Code repository started as a conversation during our June 16th meeting around designing and delivering a fully IaC solution leveraging Open Source tools which deployed a website that allowed the tracking of diabetic blood glucose levels from individuals that had been subscribed to the service. 

Terraform seems to be the most likely tool to deliver the IaC components and this repository will be used to house the deployment artificts. 

Amazon Web Services will be the deployment target, utilizing as many native services as possible

## Design
The core design will be determined through a number of collaborative sessions which go through the pros and cons of different solutions. Some of the early design decisions will be around:
- Method(s) of authentication (Cognito - define integration points)
- Front end hosting service (Cloudfront vs. EC2 vs. Amplify Console vs. Elastic Beanstalk)
- Static data servicing (DocumentDB, DymanoDB, Aurora)
- Development processes and environment (Local development or Cloud9, GitHub or CodeCommit repository, CodeStar or GitHub Project tracking, etc)
- Use CodeBuild and CodePipeline, or manually trigger updates using other methods?
- Containers (Fargate) or serverless (Lambda) for back end processing, or use simple web site with API embedded?
- Will we require SQS for message queueing between front and back end? 
- Will we utilize SNS for notification services 
- API Gateway or integrated into front end
- Creation of a Data model
- Decision around what type of configuration management to integrate (Ansible, Puppet, OpsWorks, AWS Config)
- Telemetry required

## App high level workflow

1. Welcome page with login
2. Capture authentication header
3. Query data source and provide personalized results
4. Direct to a page with personalized results displayed and method for adding, modifying, deleting new entries



