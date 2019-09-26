# Cloud Native Academy

The following course is aimed at mid to senior application developers. The course is designed to take you through the fundamental ideas and principles that are behind starting to work effectively in the cloud. In the course, we'll cover: Infrastructure As Code (with Terraform), how to launch a website on AWS S3 using Terraform, and how to create an API back-end. Throughout we'll talk about real-world considerations such as on-going maintenace, baking in security and thinking about performance. 

**Tech:** AWS (S3, Lambda), Terraform & Docker.

## Introduction

In this section we'll introduce Cloud Native Software Engineering as a discipline.

* Why learn Cloud Native?
* An Introduction to AWS
* What is AWS?
* The key AWS services

## Module 1: Setting up Infrastructure As Code

The first topic we'll cover is Infrastructure as code. By writing our infrastructure as code we'll make our life much easier when we learn the other Cloud Native topics such as launching web servers and configuring networks. 

* What is Terraform? 
* What is Infrastructure As Code
* Why Terraform vs. other provisioning tools
* [The Six Fundamental Building Blocks of Terraform?](./terraform/introduction.md)
* Your first Terraform: An S3 Bucket

## Module 2: Hosting a Website on AWS

In this section we'll build upon our previous discussion on Terraform and turn our previous S3 bucket into a website using CloudFront and Route53. 

* Introduction to DNS: What is Route53?
* Introduction to CDN's: What is CloudFront? 
* Associating Route53 with CloudFront. 
* Assigning an HTTPS with CloudFront (via ACM)

## Module 3: Building a Software Pipeline

With our Infrastructure setup for our front-end application, we'll build a software pipeline.

* What is a software pipeline? 
* Software pipeline theory. 
* Setting up a software pipeline with Github Actions

## Module 4: Building a backend API on AWS

* What is Docker? 
* Your first Container: A Web API. 
* Setting up ECR for your Containers
* Creating a pipeline for your Container
* Provisioning your Container on AWS

## Module 5: Testing your backend

* An introduction to testing theory
* How to setup backend testing

## Module 6: Backend Scaling

* What is High Availability? 
* Theory of High Availability
* How to create a cloud-based microservice

## Module 7: Operating your backend in AWS

* What is observability?
* How to setup alerts
* An introduction to logging, metrics and traces. 
* How to instrument a web API with Logging and Monitoring

## Module 78 Continuous Security & Performance

* Shifting left on Security
* What is key management? 
* Setting up AWS KMS with your application
