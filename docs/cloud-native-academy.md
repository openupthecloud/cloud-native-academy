# Cloud Native Academy

## Who is it for? 

The following course is aimed at mid to senior level software engineers. The course can act as a bolt-on to an engineering bootcamp, or acts as a framework for an existing application software engineer to become Cloud savvy. 

## Why is this course different?

* **Completeness** — Most training courses teach individual technologies or concepts and never show how different concepts work together. This is different. We show you every part of building Cloud Native applications from Infrastructure As Code, to deploying using software pipelines and monitoring your application. 

* **Software engineer-oriented** — Most training courses are either software engineering focused, or operations focused. But in the new world of cloud, software engineers need to be operationally aware too. This course gives you the tools you need to setup your operations, but from an engineering perspective. 

* **Hyper Modern** — Unlike most other training, the Cloud Native software engineering course is up-to-date with the latest and greatest trends to set you up for a great career.

* **Real Examples** — Throughout the course we'll keep referring back to one large, single use case example. Using this example you'll be able to tie in all the different concepts and ideas. 

## What we don't cover

This course is designed to teach you about architecture and infrastructure, it isn't a course on application development or design patterns. Whilst we tread a fine line into application we don't cover any. That means knowing any programming languages is entirely optional. 

## How does it work? 

The course walks you through a reference architecture. Using real-life examples to showcase all the different concepts and trade-off's such as: automated testing, observability, infrastructure as code, etc. 

[INSERT REFERENCE ARCHITECTURE]

The application comprises of a front-end, served on AWS S3, Route53 and CloudFront complete with a build, test and release pipeline. The back-end will be built on AWS Lambda, and utilises X database for persistence.

## Technology Covered

* AWS S3
* AWS Route53
* AWS Networking
* AWS Lambda

---

## Introduction

In this section we'll lay the foundations principles for Cloud Native engineering. 

* [What is Cloud Native?](https://www.thedevcoach.co.uk/what-is-a-cloud-native-software-engineer/)
* How much cloud should a software engineer know? 
* What can be considered cloud engineering? 

---

### Part 1: Getting Setup on the Cloud

**Module 1: A Cloud Services Primer**

Firstly we're going to give an introduction to the Cloud, what the Cloud is, why you'd want to use it and the advantages and disadvantages. By the end of this module you should be clear on the benefits of Cloud and be familiar with basic concepts in AWS. 

* [What and Where to Start Learning AWS as a Beginner](https://www.thedevcoach.co.uk/start-learning-aws-beginner/)
* [Setting up an AWS Cloud Account](https://www.thedevcoach.co.uk/how-to-setup-an-aws-to-experiment-and-learn/)

**Module 2: Software Pipelines**

Before we go onto infrastructure we need to discuss software pipelines. We'll do that through Github Actions. A free online CI tool that allows you to automate software pipelines easily. 

* What is a software pipeline? 
* What is container-based CI?
* An introduction to Github Actions

**Module 3: Setting up Infrastructure As Code**

Before we begin building out our application. 

The first topic we'll cover is Infrastructure as code. By writing our infrastructure as code we'll make our life much easier when we learn the other Cloud Native topics such as launching web servers and configuring networks. 

* [What is Infrastructure As Code?](https://www.thedevcoach.co.uk/infrastructure-as-code/)
* [What is Immutable Infrastructure?](https://www.thedevcoach.co.uk/what-is-immutable-infrastructure/)
* What is Terraform?
* Why Terraform vs. other provisioning tools
* [Why Learn Terraform Before Cloud Computing?](https://www.thedevcoach.co.uk/learn-terraform-before-cloud-computing/)
* [The Six Fundamental Building Blocks of Terraform?](https://www.thedevcoach.co.uk/the-six-fundamentals-of-terraform/)
* [Building an infrastructure-as-code software pipeline](https://www.thedevcoach.co.uk/setup-terraform-aws-github-actions/)
* [Your first Terraform: An S3 Bucket](https://www.thedevcoach.co.uk/terraform-github-actions/)

---

### Part 2: Building a front-end on AWS

**Module 1: Hosting a Website on AWS**

In this section we'll build upon our previous discussion on Terraform and turn our previous S3 bucket into a website using CloudFront and Route53. 

* [Introduction to S3: Making your first bucket](https://www.thedevcoach.co.uk/terraform-github-actions/)
* What you need to know about CDN's? (TTL, Refreshing)
* What is CloudFront? 
* What are HTTPS certificates (what is ACM)
* Assinging HTTPS certificates to a CloudFront distributions
* Introduction to DNS: What is Route53?
* Associating a Route53 with CloudFront. 

---

### Part 3: Building the Back-end

**Module 1: Back-End Architecture, A Primer**

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

**Module 2: Building a backend on Serverless**

* What is AWS Lambda?
* [Concepts you need to know before trying Serverless](https://www.thedevcoach.co.uk/the-6-serverless-concepts-you-need-to-know/)
* Setting up a basic AWS Lambda using Terraform
* [Getting familiar with the AWS Lambda Console](https://www.thedevcoach.co.uk/understand-aws-lambda-console/)
* [Setting up CloudWatch for logs](https://www.thedevcoach.co.uk/lambda-logging-cloudwatch/)
* [Zipping Lambda's and publishing to S3](https://www.thedevcoach.co.uk/zipped-lambda-s3-github-actions/)
* What are the events that can trigger Lambda?
* [Setting up Lambda with an ALB](https://www.thedevcoach.co.uk/setup-aws-lambda-aws-alb/)
* Setting up a DB and connecting to AWS Lambda
* [Encrypting Environment Variables With KMS](https://www.thedevcoach.co.uk/kms-aws-lambda/)

**Module 3: Building a backend with Containers**

* What is Docker? 
* Your first Container: A Web API. 
* Setting up ECR for your Containers
* Creating a pipeline for your Container
* Provisioning your Container on AWS

**Module 4: Deploying a back-end application**

* What to test in a back-end application
* Continuous Delivery / Deployment
* Unit tests, component tests, integration tests and more
* Making the case for component tests
* The perfect testing setup for a back-end Node.JS application 

**Module 5: Monitoring your backend**
* What are the different types of monitoring you can do?
* [How to structure your logs with phat-events](https://www.thedevcoach.co.uk/phat-event-logging/)
* Setting up CloudWatch dashboards
* Setting up alerts
