slide-dividers: #, ##
slidenumbers: true
slidecount: true
slide-transition: false
footer: thedevcoach.co.uk
autoscale: false

# TERRAFORM CONCEPTS

## WHAT ARE WE TALKING ABOUT?

* What Is Terraform?
* Why Learn Terraform?
* 6 Main Terraform Concepts

## WHAT IS TERRAFORM?

* Infrastructure As Code
* Command Line Utility
* Declarative

## WHY SHOULD YOU LEARN TERRAFORM?

1. Terraform helps you learn Cloud skills
1. Infrastructure skills make a Better Engineer
1. It's a great first Infrastructure tool

## TERRAFORM MAIN CONCEPTS

1. Terraform providers
1. Terraform state
1. Terraform planning & applying
1. The Language (HCL)
1. Terraform dependency resolution
1. Terraform file structure

## 1. PROVIDERS

```javascript
provider "aws" {
  region = "eu-central-1"
}
```

* To install a provider: `terraform init`

## 2. TERRAFORM STATE

```javascript
"version": 3,
"terraform_version": "0.11.14",
"modules": [{
  "resources": {
    "aws_s3_bucket.your_new_bucket": {
      "type": "aws_s3_bucket",
      "primary": {
        "id": "my-first-website-cloud-nati..."
        "attributes": {
          "bucket": "my-first-website-..."
          "bucket_domain_name": "my-fir..."
          },




⠀
```

## 3a. TERRAFORM PLAN

```javascript
Terraform will perform the following actions:

  + aws_s3_bucket.your_new_bucket
      id:                          <computed>
      acceleration_status:         <computed>
      bucket:                      "my_first_website..."
      bucket_domain_name:          <computed>
      force_destroy:               "false"
      hosted_zone_id:              <computed>
      region:                      <computed>
      request_payer:               <computed>











⠀
```

## 3b. TERRAFORM APPLYING

```javascript
Terraform will perform the following actions:

  + aws_s3_bucket.your_new_bucket
      id:                          <computed>
      acceleration_status:         <computed>
      bucket:                      "my_first_website..."
      bucket_domain_name:          <computed>
      force_destroy:               "false"
      hosted_zone_id:              <computed>
      region:                      <computed>
      request_payer:               <computed>

  Do you want to perform these actions?
    Terraform will perform the actions described above.
    Only 'yes' will be accepted to approve.







⠀
```

## 4. TERRAFORM LANGUAGE (HCL)

```javascript
terraform {
  version = "0.11.13"
}

provider "aws" {
  region = "eu-central-1"
}

resource "aws_s3_bucket" "your_new_bucket" {
  bucket = "my-first-website-clou..."
  acl    = "public-read"

  website {
    index_document = "index.html"
  }
}
```

## 5. DEPENDENCY RESOLUTION

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

## 6. FILE STRUCTURE

```
> Your Project
  > .terraform
  > terraform.tfstate
  > main.tf
  > resource_one.tf
  > resource_two.tf
```

## THATS A WRAP
