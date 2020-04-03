# Packer AWS template AMI

This project is used to create an AMI AWS with packer  and ansible

## Requirements

* Ansible
* Packer 

## Usage

Replace value aws credentials in aws_packer_template.json or create a manifest.json file to override value defined in aws_packer_template.json

```bash
packer build aws_packer_template.json
or 
packer build -var-file=manifest.json aws_packer_template.json
```

In aws console, ec2 > AMI you'll find AMI built by packer and setup by ansible. It can be used to be the base image for other EC2 instance with your custom setup 

## License

No Licence
