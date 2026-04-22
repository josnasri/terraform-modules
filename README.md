vpc module

```hcl
module "vpc" {
    source = "git::https://github.com/josnasri/terraform-modules.git"

  vpc_cidr_block    = "10.20.0.0/16"
  vpc_name          = "module-vpc"
  subnet_cidr_block = "10.20.0.0/17"
  subnet_name       = "module-subnet"
  aws_sg            = "module-sg"
  aws_igw           = "module-igw"
  aws_rt            = "module-rt"

}
```