# Cloud Native Academy

## Who is it for? 

The following course is aimed at mid to senior application developers. 

## How does it work? 

The course works by walking you through setting up a "basic" yet comprehensive cloud-based web application. The application will comprise of a front-end, served on AWS S3, Route53 and CloudFront complete with a build, test and release pipeline. 

The back-end will be built on AWS Lambda

As we cover each aspect, we'll discuss pro's, con's architectural decisions and trade-off's. No stone will be left underturned, and by the end you'll have a comprehensive understanding of modern application design, and creation using Cloud Native technologies. 

## Why this course? 

This course is different because unlike others, which only show you one technology, we'll show you how you can fit all the pieces together to create a full, working application. Sparing no details you'll understand how to setup your application, how to script your infrastructure, how to secure your application, and how to setup deployments on your infrastructure. 

**Tech:** AWS (S3, Lambda), Terraform & Docker.

## Introduction

In this section we'll introduce Cloud Native Software Engineering as a discipline.

* [What is Cloud Native?](https://www.thedevcoach.co.uk/what-is-a-cloud-native-software-engineer/)
* The Full Stack Engineer: Fact or fiction? 
* What makes Cloud Native engineering different
* Why Cloud Native is the future of Software Engineering
* Tools of the Cloud Native Engineer
* [Setting up an AWS Cloud Account](https://www.thedevcoach.co.uk/how-to-setup-an-aws-to-experiment-and-learn/)

### Module 1: A Cloud Services Primer

A quick introduction to AWS, and the AWS main services

* [What you need to know before learning cloud (serverless)](https://www.thedevcoach.co.uk/the-6-serverless-concepts-you-need-to-know/)
* What is AWS?
* The AWS key services landscape
* What are the main AWS services?

### Module 2: Setting up Infrastructure As Code

The first topic we'll cover is Infrastructure as code. By writing our infrastructure as code we'll make our life much easier when we learn the other Cloud Native topics such as launching web servers and configuring networks. 

* [Why Learn Terraform Before Cloud Computing?](https://www.thedevcoach.co.uk/learn-terraform-before-cloud-computing/)
* What is Terraform? 
* What is Infrastructure As Code
* Why Terraform vs. other provisioning tools
* [The Six Fundamental Building Blocks of Terraform?](https://www.thedevcoach.co.uk/the-six-fundamentals-of-terraform/)
* Your first Terraform: An S3 Bucket

### Module 3: Hosting a Website on AWS

In this section we'll build upon our previous discussion on Terraform and turn our previous S3 bucket into a website using CloudFront and Route53. 

* Introduction to DNS: What is Route53?
* Introduction to CDN's: What is CloudFront? 
* Associating Route53 with CloudFront. 
* Assigning an HTTPS with CloudFront (via ACM)

### Module 4: Building a Software Pipeline

With our Infrastructure setup for our front-end application, we'll build a software pipeline.

* What is a software pipeline? 
* Software pipeline theory. 
* Setting up a software pipeline with Github Actions

### Module 5: Building a backend API on Serverless

* Building a Distributed system, what you need to know. 
* Understanding the basics of AWS Lambda
* [Zipping Lambda's and publishing to S3](https://www.thedevcoach.co.uk/zipped-lambda-s3-github-actions/)
* What is a Load Balancer and why would you need one? 
* [Setting up Lambda with an ALB](https://www.thedevcoach.co.uk/setup-aws-lambda-aws-alb/)
* Setting up a DB and connecting to AWS Lambda

### Module 6: Building a backend API With Containers

* What is Docker? 
* Your first Container: A Web API. 
* Setting up ECR for your Containers
* Creating a pipeline for your Container
* Provisioning your Container on AWS

### Module 7: Testing your application

* An introduction to testing theory
* How to setup backend testing

### Module 8: Backend Scaling

* What is High Availability? 
* Theory of High Availability
* How to create a cloud-based microservice

### Module 9: Operating your backend in AWS

* What is observability?
* How to setup alerts
* An introduction to logging, metrics and traces. 
* How to instrument a web API with Logging and Monitoring

### Module 10: Continuous Security & Performance

* Shifting left on Security
* What is key management? 
* Setting up AWS KMS with your application
