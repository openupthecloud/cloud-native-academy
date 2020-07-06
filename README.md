# Cloud Native Academy (CNA)

The Cloud Native Academy (CNA) is a free cloud native learning course composed of individual articles that have been written on [The Dev Coach](http://thedevcoach.co.uk/) blog. My intention in the future is to make the articles into some form of video course, but for now you can consider this the beta. The following course (and it's structure) is designed to give software engineers that are learning cloud engineering structure and direction for their learning. 

CNA is primarily aimed at mid to senior experience software engineers but would work equally well as a supplement or follow-up to a software engineering bootcamp. Engineers who already have experience writing code, but want to broaden their experience to also include cloud computing concepts. 

Interested to learn Cloud Native Software Engineering? Read on. 

## Why Is The Cloud Native Academy Different?

You might be wondering: "What's different about this 'course' compared to all the free information and courses that currently exist on the internet?". Let me address that question...

* **Completeness** — Many learning resources teach only individual technologies or concepts and don't show how the different concepts work together. CNA shows you every part of building Cloud Native applications from Infrastructure As Code, to deploying using software pipelines and monitoring your application. 

* **Software engineer-oriented** — Most training courses are either software engineering focused, or operations focused. But in the new world of cloud, software engineers need to be operationally aware, and code skilled. gives you the tools you need to setup your operations, but from an engineering perspective. 

* **Ultra Modern** — Unlike most other training, the Cloud Native software engineering course is at the cutting edge of the latest cloud native trends. This isn't an old curriculm that's been running for years, it's based on the lastest thinking and tools.

## Technology Covered

* AWS, S3, Route53, Networking, Lambda, Node.JS

## Cloud Native Academy Email Courses

I am currently in the process of converting each module of the CNA into stand-alone email courses to be taken separately, you can see the current email courses on the [courses page](http://courses.thedevcoach.co.uk/) ([AWS Course](https://aws.thedevcoach.co.uk/) | [Terraform Course](https://terraform.thedevcoach.co.uk/)
| [Lambda Course](https://lambda.thedevcoach.co.uk/))

---

## Introduction

In this section we'll lay the foundations principles for Cloud Native engineering. 

* [What is Cloud Native?](https://www.thedevcoach.co.uk/what-is-a-cloud-native-software-engineer/)
* How much cloud should a software engineer know? 
* What can be considered cloud engineering? 

---

## Part 1: Getting Setup on the Cloud

### Module 1.1: Cloud Services, A Primer

**Enroll On Email Course:** ✉️ [AWS Email Course](https://aws.thedevcoach.co.uk/)

* [What and Where to Start Learning AWS as a Beginner](https://www.thedevcoach.co.uk/start-learning-aws-beginner/)
* [Setting up an AWS Cloud Account](https://www.thedevcoach.co.uk/how-to-setup-an-aws-to-experiment-and-learn/)
* [How to setup your AWS account to experiment and learn](https://www.thedevcoach.co.uk/how-to-setup-an-aws-to-experiment-and-learn/)
* [Using AWS access keys](https://www.thedevcoach.co.uk/aws-access-keys/)

### Module 1.2: Software Pipelines

* What is a software pipeline? 
* What is container-based CI?
* An introduction to Github Actions
* How many software pipelines should you have?

### Module 1.3: Setting up Infrastructure As Code (Using Terraform)

**Enroll On Email Course:** ✉️ [Terraform Email Course](https://terraform.thedevcoach.co.uk/)

* Why is Terraform so popular?
* [What is Infrastructure As Code?](https://www.thedevcoach.co.uk/infrastructure-as-code/)
* [What is Immutable Infrastructure?](https://www.thedevcoach.co.uk/what-is-immutable-infrastructure/)
* [Declarative Infrastructure As Code](https://www.thedevcoach.co.uk/declarative-vs-imperative-infra/)
* [What is Terraform?](https://www.thedevcoach.co.uk/what-is-terraform/)
* Terraform vs CloudFormation vs etc. 
* [Why Learn Terraform Before Cloud Computing?](https://www.thedevcoach.co.uk/learn-terraform-before-cloud-computing/)
* [The Six Fundamentals Of Terraform](https://www.thedevcoach.co.uk/the-six-fundamentals-of-terraform/)
* [The Six Fundamental Building Blocks of Terraform?](https://www.thedevcoach.co.uk/the-six-fundamentals-of-terraform/)
* [Building an infrastructure-as-code software pipeline](https://www.thedevcoach.co.uk/setup-terraform-aws-github-actions/)
* [Setting Up Terraform With Github Actions](https://www.thedevcoach.co.uk/setup-terraform-aws-github-actions/)
* [Your first Terraform: An S3 Bucket](https://www.thedevcoach.co.uk/terraform-github-actions/)
* [10 Terraform Best Practices](https://www.thedevcoach.co.uk/terraform-best-practices/)
* Managing & Understanding Terraform State

***Extra Credits**

* [Migrating Manually Created Infrastructure](https://www.thedevcoach.co.uk/refactor-existing-infrastructure-with-terraform/)
* [Understanding Terraform Modules](https://www.thedevcoach.co.uk/terraform-modules-tutorial/)

---

## Part 2: Building a front-end on AWS

### Module 2.1: Hosting a Website on AWS

* [Introduction to S3: Making your first bucket](https://www.thedevcoach.co.uk/terraform-github-actions/)
* What you need to know about CDN's? (TTL, Refreshing)
* What is CloudFront? 
* What are HTTPS certificates (what is ACM)
* Assigning HTTPS certificates to a CloudFront distributions
* Introduction to DNS: What is Route53?
* Associating a Route53 with CloudFront. 

---

## Part 3: Building the Back-end

### Module 3.1: Back-End Architecture

* Overview of back-end cloud tech: Serverless, Containers, Queues, Load Balancers, Gateways, Encryption.
* * How Tech Companies Organise Their Cloud Accounts
* Service Communication Methods: Asyncronous vs Point-To-Point Architecture?
  * [Building asynchronous architectures with SQS](https://www.thedevcoach.co.uk/aws-sqs-and-lambda/)
* What is a load balancer? 

### Module 3.2: Building A Back-End With Serverless (Lambda)

**Enroll On Email Course:** ✉️ [Lambda Email Course](https://lambda.thedevcoach.co.uk/)

* What Is Serverless?
* What is AWS Lambda?
* Serverless vs Functions vs FaaS vs ...: What's the difference?
* Serverless & Events: What Events Does AWS Lambda Integrate With?
* Creating A Lambda Function (Using Terraform & Github Actions)
* [Concepts To Know Before Using Serverless](https://www.thedevcoach.co.uk/the-6-serverless-concepts-you-need-to-know/)
* [Serverless Frameworks / Approaches Compared](https://www.thedevcoach.co.uk/serverless-approaches-comparison/)
* Difference in Serverless between the Cloud Providers
* [Misconceptions of Serverless & Lambda](https://www.thedevcoach.co.uk/misconceptions-serverless-aws-lambda/)
* [Understanding the Lambda Console](https://www.thedevcoach.co.uk/understand-aws-lambda-console/)
* [Setup CloudWatch Logs with AWS Lambda](https://www.thedevcoach.co.uk/lambda-logging-cloudwatch/)
* [Good Serverless beginner projects](https://www.thedevcoach.co.uk/serverless-beginner-project/)
* [Setup an ALB with Lambda](https://www.thedevcoach.co.uk/setup-aws-lambda-aws-alb/)
* Setting up a DB and connecting to AWS Lambda
* Setting up a basic AWS Lambda using Terraform

***Extra Credits**
* [Encrypting Environment Variables With KMS](https://www.thedevcoach.co.uk/kms-aws-lambda/)
* [How to use Lambda With SQS](https://www.thedevcoach.co.uk/aws-sqs-and-lambda/)
* [How to schedule a Lambda invocation](https://www.thedevcoach.co.uk/terraform-lambda-scheduled-event/)

### Module 3.3: Building a backend with Containers

* What is Docker? 
* Your first Container: A Web API. 
* Setting up ECR for your Containers
* Creating a pipeline for your Container
* Provisioning your Container on AWS

---

## Part 4: Deploying a back-end application

* What to test in a back-end application
* Continuous Delivery / Deployment
* Unit Tests, Component Tests, Integration Tests & More.
* Making The Case For Component Tests
* The perfect testing setup for a back-end Node.JS application 

---

## Part 5: Monitoring your backend

* What are the different types of monitoring you can do?
* [How to structure your logs with phat-events](https://www.thedevcoach.co.uk/phat-event-logging/)
* Setting up CloudWatch dashboards
* What are alerts and why are they useful?
* What is on-call culture?
