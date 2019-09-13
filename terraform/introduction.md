slide-dividers: #, ##
slidenumbers: true
slidecount: true
slide-transition: false
footer: thedevcoach.co.uk
autoscale: false


# [fit] INTRODUCTION TO TERRAFORM

# WHO AM I?

* Lou Bichard!
* Cloud Native Software Engineer
* [thedevcoach.co.uk]()
* [thedevcoach.co.uk/newsletter](thedevcoach.co.uk/newsletter)

Twitter: **@loujaybee**
Website: **thedevcoach.co.uk**

![left](../lou.jpeg)

## AGENDA

* What is Terraform?
* Why Terraform beats all competition
* Why Terraform is very cool
* An example creating some S3 infrastructure with Terraform

## WHY TERRAFORM BEATS ALL COMPETITION

* Terraform is Technology Agnostic
* Terraform knowledge transfers between cloud providers


## 3 PRINCIPLES OF TERRAFORM

There are three core areas to know when it comes to Terraform...

* **State** — What Terraform knows about your infrastructure
* **Code** — What you want your infrastructure to look like
* **Infra** — The actual current state of your infrastructure

## WHAT DOES STATE LOOK LIKE?

```javascript
 {
     "modules": [
        {
            "outputs": {},
            "resources": {
                "aws_lambda_alias.env_alias": {
                    "type": "aws_lambda_alias",
                    "primary": {
                        "id": "arn:aws:lambda:eu-west-2:082876741967:function:l
                        "attributes": {
                            "arn": "arn:aws:lambda:eu-west-2:082876741967:funct
                            "description": "Version of lambda used on elizabeth line",
                            "function_name": "lambda-dazn-tube-auth0-authorizer-elizabeth",
                            "function_version": "$LATEST",
                            "id": "arn:aws:lambda:eu-west-2:082876741967:functi
                            "invoke_arn": "arn:aws:apigateway:eu-west-2:lambda:
                            "name": "elizabeth",
                            "routing_config.#": "0"
```


## WHAT IS TERRAFORM

* An Infrastructure-As-Code CLI[^1].
* Does stuff

[^1]: This not what I'd recommend

## WHAT DOES TERRAFORM LOOK LIKE?

[.code-highlight: 1-4]
[.code-highlight: 6-10]

```ruby
terraform {
  version = "0.11.13"
  backend "s3"    {}
}

provider "aws" {
  region              = "eu-central-1"
  version             = "~> 2.26"
  allowed_account_ids = ["${var.account_id}"]
}
```

## WHAT IS A TERRAFORM PROVIDER?

* Allows you to write code for a specific platform

## RUNNING A TERRAFORM COMMAND

```bash
terraform apply
```

## Other Stuff

Content
