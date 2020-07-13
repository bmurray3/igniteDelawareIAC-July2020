# igniteDelawareIAC-July2020

## Purpose
> This Ignite Delaware Infrastructure as Code repository started as a conversation during our June 16th meeting around designing and delivering a fully IaC solution leveraging Open Source tools which deployed a website that allowed the tracking of diabetic blood glucose levels from individuals that had been subscribed to the service. 

> Terraform seems to be the most likely tool to deliver the IaC components and this repository will be used to house the deployment artificts. 

> Amazon Web Services will be the deployment target, utilizing as many native services as possible

## Design
> The core design will be determined through a number of collaborative sessions which go through the pros and cons of different solutions. Some of the early design decisions will be around:
- Method(s) of authentication (Cognito - define integration points)
- Front end hosting service (Cloudfront vs. EC2 vs. Amplify Console)
- Static data servicing (DocumentDB, DymanoDB, Aurora)
- Development processes and environment (Local development or Cloud9, GitHub or CodeCommit repository, CodeStar or GitHub Project tracking, etc)
- Containers (Fargate) or serverless (Lambda)
- API Gateway or integrated into front end
- Creation of a Data model
- 
