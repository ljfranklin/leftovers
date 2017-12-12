# Leftovers

Clean up orphaned IAAS resources.

## Why you might be here?
- You `terraform apply`'d way back when and lost your `terraform.tfstate`
- You used the console or cli to create some infrastructure and want to clean up
- Your acceptance tests in CI failed, the container disappeared, and
infrastructure resources were tragically orphaned

## AWS
### Currently deleting
- iam instance profiles (& detaching roles)
- iam roles
- iam role policies
- iam server certificates
- ec2 volumes
- ec2 tags
- ec2 key pairs
- ec2 instances
- ec2 security groups
- ec2 vpcs
- elb load balancers

### Upcoming
- iam group policies
- iam user policies
- elbv2 load balancers
- ec2 eips
- ec2 enis
- s3 buckets

## GCP
### Upcoming
- compute disks
- compute health checks
- compute vm instances
- compute vm instance groups
- compute vm instance templates
- compute snapshots
- compute images