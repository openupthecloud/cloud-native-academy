slide-dividers: #, ##
slidenumbers: true
slidecount: true
slide-transition: false
footer: thedevcoach.co.uk
autoscale: false

# LEARNING THE FUNDAMENTALS OF TERRAFORM (PART 1)

 — in under an hour —

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
* Why should you learn Terraform?
* Why Terraform instead of Chef, Ansible, [insert tool]?
* Main Terraform concepts (planning, applying, state etc)

## WHAT IS TERRAFORM?

* Infrastructure-as-code tool
* Client-based
* Provisioning
* Declarative

## WHY SHOULD YOU LEARN TERRAFORM?

1. It helps you learn other cloud tools
1. Broader skills make for a better engineer
1. It's the best current provisioning tool

## WHY TERRAFORM INSTEAD OF ANSIBLE, CHEF, PUPPET, [INSERT TOOL]?

* A standard langauge
* Scripting of non-cloud resources
* Reduced impact of lock-in

## TERRAFORM MAIN FEATURES

1. The Language (HCL)
1. Terraform planning & applying
1. Terraform state
1. Terraform dependency resolution
1. Terraform file structure
1. Terraform providers

## SOME EXAMPLE TERRAFORM

[.code-highlight: 1-20]
[.code-highlight: 1-3]
[.code-highlight: 4-7]
[.code-highlight: 8-20]


```javascript
terraform {
  version = "0.11.13"
}

provider "aws" {
  region = "eu-central-1"
}

resource "aws_s3_bucket" "your_new_bucket" {
  bucket = "my-first-website-cloud-native-website"
  acl    = "public-read"

  website {
    index_document = "index.html"
  }
}
```

## TERRAFORM LANGUAGE (HCL)

[.code-highlight: 1-10]
[.code-highlight: 1]
[.code-highlight: 2-6]

```javascript
terraform_command "provider_resource_name" "resource_name" {
   "option_1": "option_1",
   "option_2": "option_2",
   "option_3": "option_3",
   "option_4": "option_4",
   "option_5": "option_5",
}
```

## TERRAFORM PLAN

[.code-highlight: 1-40]
[.code-highlight: 5]
[.code-highlight: 8]
[.code-highlight: 9]
[.code-highlight: 13]

```javascript
Lou > terraform plan

An execution plan has been generated and is shown below.
Resource actions are indicated with the following symbols:
  + create

Terraform will perform the following actions:

  + aws_s3_bucket.your_new_bucket
      id:                          <computed>
      acceleration_status:         <computed>
      bucket:                      "my_first_website_cloud_native_website_${random_string.random.result}"
      bucket_domain_name:          <computed>
      force_destroy:               "false"
      hosted_zone_id:              <computed>
      region:                      <computed>
      request_payer:               <computed>
```

## TERRAFORM APPLYING

[.code-highlight: 0-25]
[.code-highlight: 18-25]

```javascript
Lou > terraform plan

An execution plan has been generated and is shown below.
Resource actions are indicated with the following symbols:
  + create

Terraform will perform the following actions:

  + aws_s3_bucket.your_new_bucket
      id:                          <computed>
      acceleration_status:         <computed>
      bucket:                      "my_first_website_cloud_native_website_${random_string.random.result}"
      bucket_domain_name:          <computed>
      force_destroy:               "false"
      hosted_zone_id:              <computed>
      region:                      <computed>
      request_payer:               <computed>

  Do you want to perform these actions?
    Terraform will perform the actions described above.
    Only 'yes' will be accepted to approve.
```

## TERRAFORM STATE

```javascript
"version": 3,
"terraform_version": "0.11.14",
"modules": [
    {
        "resources": {
            "aws_s3_bucket.your_new_bucket": {
                "type": "aws_s3_bucket",
                "primary": {
                    "id": "my-first-website-cloud-native-website-my-lovely-bucket",
                    "attributes": {
                        "bucket": "my-first-website-cloud-native-website-my-lovely-bucket",
                        "bucket_domain_name": "my-first-website-cloud-native-website-my-lovely-bucket.s3.amazonaws.com",
                    },
```

* Is an undocumented API
* Represents what Terraform is managing
* It's just a file, if it's a backend, it's the same file but on remote

## DEPENDENCY RESOLUTION

```javascript
digraph {
	compound = "true"
	newrank = "true"
	subgraph "root" {
		"[root] aws_s3_bucket.your_new_bucket" [label = "aws_s3_bucket.your_new_bucket", shape = "box"]
		"[root] provider.aws" [label = "provider.aws", shape = "diamond"]
		"[root] aws_s3_bucket.your_new_bucket" -> "[root] provider.aws"
		"[root] meta.count-boundary (count boundary fixup)" -> "[root] aws_s3_bucket.your_new_bucket"
		"[root] provider.aws (close)" -> "[root] aws_s3_bucket.your_new_bucket"
		"[root] root" -> "[root] meta.count-boundary (count boundary fixup)"
		"[root] root" -> "[root] provider.aws (close)"
	}
}
```

* Terraform works out how to create your resources
* It's how you link one resource to the next

## FILE STRUCTURE

```
> Your Project
  > .terraform
  > terraform.tfstate
  > main.tf
  > resource_one.tf
  > resource_two.tf
```

* Terraform is clever, define resources in any order
* Subfolders are modules

## PROVIDERS

```javascript
provider "aws" {
  region = "eu-central-1"
}
```

* Same syntax as resources
* A provider can be put anywhere
* To install a provider: `terraform init`

## THATS A WRAP

* All we're going to cover today!
* Next up: A working tutorial!
