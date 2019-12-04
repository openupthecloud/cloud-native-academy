# Cloud Native Academy

## Who is it for? 

The following course is aimed at mid to level software engineers. The course acts as a bolt-on to an engineering bootcamp, or acts as a framework to help a software engineer to understand which parts of application development they are weak on. 

## Why is this course different?

* **Completeness** — Most courses teach individual technologies or concepts and never show how different concepts work together, such as how we manage infrastructure deployments alongside code deployments or how to structure infrastructure as code projects.

* **Software engineer-oriented** — Most courses are either software engineering focused, or operations focused. But in the new world of cloud, software engineers have to be operationally aware. This course views operations from an engineering perspective. 

* **Real Examples** — The course will go through one, large real-world example. A full application, with a front-end and back-end.

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

An introduction to AWS, and the main services.

* What is AWS? 
* [What and Where to Start Learning AWS as a Beginner](https://www.thedevcoach.co.uk/start-learning-aws-beginner/)
* [Setting up an AWS Cloud Account](https://www.thedevcoach.co.uk/how-to-setup-an-aws-to-experiment-and-learn/)

**Module 2: Setting up Infrastructure As Code**

Before we begin building out our application. 

The first topic we'll cover is Infrastructure as code. By writing our infrastructure as code we'll make our life much easier when we learn the other Cloud Native topics such as launching web servers and configuring networks. 

* [What is Infrastructure As Code?](https://www.thedevcoach.co.uk/infrastructure-as-code/)
* [What is immutable infrastructure?](https://www.thedevcoach.co.uk/what-is-immutable-infrastructure/)
* [Why Learn Terraform Before Cloud Computing?](https://www.thedevcoach.co.uk/learn-terraform-before-cloud-computing/)
* What is Terraform? 
* Why Terraform vs. other provisioning tools
* [The Six Fundamental Building Blocks of Terraform?](https://www.thedevcoach.co.uk/the-six-fundamentals-of-terraform/)
* Your first Terraform: An S3 Bucket
* Setting up a Terraform pipeline in Github Actions
* Best practices for a Terraform project (alongside code, etc)
* How to setup Terraform repo's with remote state and link them

---

### Part 2: Hosting A Website on AWS

**Module 1: Hosting a Website on AWS**

In this section we'll build upon our previous discussion on Terraform and turn our previous S3 bucket into a website using CloudFront and Route53. 

* Introduction to S3: Making your first bucket.
* What you need to know about CDN's? (TTL, Refreshing)
* What is CloudFront? 
* What are HTTPS certificates (what is ACM)
* Assinging HTTPS certificates to a CloudFront distributions
* Introduction to DNS: What is Route53?
* Associating a Route53 with CloudFront. 

**Module 2: Deploying a front-end application**

With our Infrastructure setup for our front-end application, we'll build a software pipeline.

* What is a software pipeline? 
* Software pipeline theory. 
* Setting up a front-end software pipeline.
* How to test a front-end application.
* Best practices for monitoring on a front-end application in S3
* Setting up a software pipeline with Github Actions

---

### Part 3: Building the Back-end

**Module 1: Back-End Architecture, A Primer**

* What is a distributed system?
* Considerations in a distributed systems world.
* Serverless or Containers: How to choose? 
* Understanding high availability.
* Why observability is important.
* How to instrument a back-end microservice (error handling, error codes, etc).

**Module 2: Building a backend on Serverless**

* [Concepts you need to know before trying Serverless](https://www.thedevcoach.co.uk/the-6-serverless-concepts-you-need-to-know/)
* Understanding the basics of AWS Lambda
* [Setting up CloudWatch for logs](https://www.thedevcoach.co.uk/lambda-logging-cloudwatch/)
* [Zipping Lambda's and publishing to S3](https://www.thedevcoach.co.uk/zipped-lambda-s3-github-actions/)
* What is a Load Balancer and why would you need one? 
* [Setting up Lambda with an ALB](https://www.thedevcoach.co.uk/setup-aws-lambda-aws-alb/)
* Setting up a DB and connecting to AWS Lambda

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
