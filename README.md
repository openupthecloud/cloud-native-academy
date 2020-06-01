# Cloud Native Academy (CNA)

The Cloud Native Academy (CNA) is a free cloud native learning course composed of individual articles that have been written on [The Dev Coach](http://thedevcoach.co.uk/) blog. The following course and it's structure is designed to give software engineers learning cloud engineering the structure and direction they need around their learning. 

CNA is primarily aimed at mid to senior experience software engineers but would work equally well as a supplement or follow-up to a software engineering bootcamp. Engineers who already have experience writing code, but want to broaden their experience to also include cloud computing concepts. 

## Why Is The Cloud Native Academy Different?

* **Completeness** — Many learning resources teach only individual technologies or concepts and don't show how the different concepts work together. The CNA is different. CNA shows you every part of building Cloud Native applications from Infrastructure As Code, to deploying using software pipelines and monitoring your application. 

* **Software engineer-oriented** — Most training courses are either software engineering focused, or operations focused. But in the new world of cloud, software engineers need to be operationally aware, and code skilled. gives you the tools you need to setup your operations, but from an engineering perspective. 

* **Hyper Modern** — Unlike most other training, the Cloud Native software engineering course is up-to-date with the latest and greatest trends to set you up for a great career.

* **Real Examples** — Throughout CNA we'll keep referring back to one large, single use case example. Using this example you'll be able to tie in all the different concepts and ideas. 

## What CNA Isn't

This course is designed to teach you about architecture and infrastructure, it isn't a course on application development or design patterns. Whilst we tread a fine line into application we don't cover any. That means knowing any programming languages is entirely optional.

## Technology Covered

* AWS S3
* AWS Route53
* AWS Networking
* AWS Lambda

## Cloud Native Academy Email Courses

I am currently in the process of converting each module of the CNA into stand-alone email courses to be taken separately, you can see the current email courses on the [courses page](http://courses.thedevcoach.co.uk/). 

---

## Introduction

In this section we'll lay the foundations principles for Cloud Native engineering. 

* [What is Cloud Native?](https://www.thedevcoach.co.uk/what-is-a-cloud-native-software-engineer/)
* How much cloud should a software engineer know? 
* What can be considered cloud engineering? 

---

## Part 1: Getting Setup on the Cloud

### Module 1: Cloud Services, A Primer

Firstly we're going to give an introduction to the Cloud, what the Cloud is, why you'd want to use it and the advantages and disadvantages. By the end of this module you should be clear on the benefits of Cloud and be familiar with basic concepts in AWS. 

* [What and Where to Start Learning AWS as a Beginner](https://www.thedevcoach.co.uk/start-learning-aws-beginner/)
* [Setting up an AWS Cloud Account](https://www.thedevcoach.co.uk/how-to-setup-an-aws-to-experiment-and-learn/)
* [How to setup your AWS account to experiment and learn](https://www.thedevcoach.co.uk/how-to-setup-an-aws-to-experiment-and-learn/)
* [Using AWS access keys](https://www.thedevcoach.co.uk/aws-access-keys/)

### Module 2: Software Pipelines

Before we go onto infrastructure we need to discuss software pipelines. We'll do that through Github Actions. A free online CI tool that allows you to automate software pipelines easily. 

* What is a software pipeline? 
* What is container-based CI?
* An introduction to Github Actions

### Module 3: Setting up Infrastructure As Code**

Before we begin building out our application. 

The first topic we'll cover is Infrastructure as code. By writing our infrastructure as code we'll make our life much easier when we learn the other Cloud Native topics such as launching web servers and configuring networks. 

* [What is Infrastructure As Code?](https://www.thedevcoach.co.uk/infrastructure-as-code/)
* [What is Immutable Infrastructure?](https://www.thedevcoach.co.uk/what-is-immutable-infrastructure/)
* [What is Terraform?](https://www.thedevcoach.co.uk/what-is-terraform/)
* [Why Learn Terraform Before Cloud Computing?](https://www.thedevcoach.co.uk/learn-terraform-before-cloud-computing/)
* [The Six Fundamental Building Blocks of Terraform?](https://www.thedevcoach.co.uk/the-six-fundamentals-of-terraform/)
* [Building an infrastructure-as-code software pipeline](https://www.thedevcoach.co.uk/setup-terraform-aws-github-actions/)
* [Your first Terraform: An S3 Bucket](https://www.thedevcoach.co.uk/terraform-github-actions/)

#### What is Terraform?

* [What is Infrastructure As Code?](https://www.thedevcoach.co.uk/infrastructure-as-code/)
* [Learn Terraform Before Cloud](https://www.thedevcoach.co.uk/learn-terraform-before-cloud-computing/)
* [What is Terraform?](https://www.thedevcoach.co.uk/what-is-terraform/)
* Terraform vs CloudFormation vs etc. 
* [Declarative Infrastructure As Code](https://www.thedevcoach.co.uk/declarative-vs-imperative-infra/)
* [The Six Fundamentals Of Terraform](https://www.thedevcoach.co.uk/the-six-fundamentals-of-terraform/)

#### Get Hands On With Terraform 

* [Setting Up Terraform With Github Actions](https://www.thedevcoach.co.uk/setup-terraform-aws-github-actions/)
* [Create an S3 website using Terraform](https://www.thedevcoach.co.uk/terraform-github-actions/)
* Managing & Understanding Terraform State
* [10 Terraform Best Practices](https://www.thedevcoach.co.uk/terraform-best-practices/)

#### Advanced Terraform

* [Migrating Manually Created Infrastructure](https://www.thedevcoach.co.uk/refactor-existing-infrastructure-with-terraform/)
* [Understanding Terraform Modules](https://www.thedevcoach.co.uk/terraform-modules-tutorial/)


---

## Part 2: Building a front-end on AWS

### Module 1: Hosting a Website on AWS

In this section we'll build upon our previous discussion on Terraform and turn our previous S3 bucket into a website using CloudFront and Route53. 

* [Introduction to S3: Making your first bucket](https://www.thedevcoach.co.uk/terraform-github-actions/)
* What you need to know about CDN's? (TTL, Refreshing)
* What is CloudFront? 
* What are HTTPS certificates (what is ACM)
* Assinging HTTPS certificates to a CloudFront distributions
* Introduction to DNS: What is Route53?
* Associating a Route53 with CloudFront. 

---

## Part 3: Building the Back-end

### Module 1: Back-End Architecture, A Primer

In this module we'll cover the different options you've got for building a back-end. We'll cover the two main patterns for building back-end applications: container-based and serverless-based. After this module we'll create a back-end in both a Container based solution, and also a Serverless based solution. 

* What is a Distributed System?
* Considerations in a distributed systems world.
* Serverless or Containers: How do you choose? 
* Understanding high availability.
* Why observability is important.
* What is an asyncronous architecture?
* [Building asynchronous architectures with SQS](https://www.thedevcoach.co.uk/aws-sqs-and-lambda/)
* What is a load balancer? 
* How to instrument a back-end microservice (error handling, error codes, etc).

### Module 2: Building a backend on Serverless

* Serverless: An introduction
* FaaS vs Serverless vs Serverless Inc
* Characteristics of Serverless
* What is AWS Lambda?
* Serverless vs Functions vs FaaS vs ...: What's the difference?
* Serverless Framework: An Overview.
* Difference in Serverless between the Cloud Providers
* [Misconceptions of Serverless & Lambda](https://www.thedevcoach.co.uk/misconceptions-serverless-aws-lambda/)
* [Good Serverless beginner projects](https://www.thedevcoach.co.uk/serverless-beginner-project/)
* [Serverless frameworks / approaches compared](https://www.thedevcoach.co.uk/serverless-approaches-comparison/)
* [Understanding the Lambda Console](https://www.thedevcoach.co.uk/understand-aws-lambda-console/)
* [Setup CloudWatch Logs with AWS Lambda](https://www.thedevcoach.co.uk/lambda-logging-cloudwatch/)
* [Concepts you need to know before trying Serverless](https://www.thedevcoach.co.uk/the-6-serverless-concepts-you-need-to-know/)
* [Setup an ALB with Lambda](https://www.thedevcoach.co.uk/setup-aws-lambda-aws-alb/)
* [Encrypting Environment Variables With KMS](https://www.thedevcoach.co.uk/kms-aws-lambda/)
* [How to use Lambda With SQS](https://www.thedevcoach.co.uk/aws-sqs-and-lambda/)
* [How to schedule a Lambda invocation](https://www.thedevcoach.co.uk/terraform-lambda-scheduled-event/)
* Creating A Lambda Function (Using Terraform & Github Actions)
* What are the events that can trigger Lambda?
* Setting up a DB and connecting to AWS Lambda
* Setting up a basic AWS Lambda using Terraform

### Module 3: Building a backend with Containers

* What is Docker? 
* Your first Container: A Web API. 
* Setting up ECR for your Containers
* Creating a pipeline for your Container
* Provisioning your Container on AWS

### Module 4: Deploying a back-end application

* What to test in a back-end application
* Continuous Delivery / Deployment
* Unit tests, component tests, integration tests and more
* Making the case for component tests
* The perfect testing setup for a back-end Node.JS application 

### Module 5: Monitoring your backend
* What are the different types of monitoring you can do?
* [How to structure your logs with phat-events](https://www.thedevcoach.co.uk/phat-event-logging/)
* Setting up CloudWatch dashboards
* Setting up alerts

