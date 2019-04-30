# terraform-aws-microsoftad
Create a Microsoft Active Directory AWS Directory Service

# Overview

Creates Microsoft AD AWS Directory Service

## Requirements

This module requires Terraform version `0.10.x` or newer.

## Dependencies

This module depends on a correctly configured [AWS Provider](https://www.terraform.io/docs/providers/aws/index.html) in your Terraform codebase.

## Usage

```
module "ad" {
    source = "neillturner/microsoftad/aws"
    version = "0.1.0"
    domain_name     = "aws.example.com"
    short_name      = "corp"
    computer_ou     = "ou=aws,dc=example,dc=com"
    edition         = "Standard"
    admin_password  = "secret"
    vpc_id          = vpc-xxxxxx"
    subnet_ids      = "subnet-yyyyyyyyy"
  }
```
## variables
