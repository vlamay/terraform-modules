# Terraform Modules

Reusable Terraform modules for VPC, EKS, RDS, S3 with comprehensive documentation.

## Overview

This repository contains production-ready Terraform modules for AWS infrastructure:

- **VPC Module**: Complete VPC setup with subnets, NAT gateways, and routing
- **EKS Module**: Kubernetes cluster on AWS with security best practices
- **RDS Module**: Managed database instances with high availability
- **S3 Module**: Secure S3 buckets with encryption and versioning

## Structure

```
.
├── modules/
│   ├── vpc/           # VPC module
│   ├── eks/           # EKS module
│   ├── rds/           # RDS module
│   └── s3/            # S3 module
├── examples/          # Usage examples
└── docs/             # Documentation
```

## Requirements

- Terraform >= 1.0
- AWS Provider >= 4.0

## Usage

```hcl
module "vpc" {
  source = "github.com/vlamay/terraform-modules//modules/vpc"
  
  name = "production-vpc"
  cidr = "10.0.0.0/16"
  
  azs = ["us-east-1a", "us-east-1b"]
}
```

## Features

- ✅ Production-ready modules
- ✅ Security best practices
- ✅ Comprehensive documentation
- ✅ Usage examples
- ✅ Multi-region support

## Contributing

Contributions are welcome! Please read CONTRIBUTING.md for guidelines.

## License

MIT License
