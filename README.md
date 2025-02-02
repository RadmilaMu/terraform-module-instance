# terraform-module-instance

```hcl
module "instance" {
  source  = "RadmilaMu/instance./module"
  version = "1.0.0"
  region = "us-east-2"   # Replace with your values
  instance_type = "t2.micro"  # Replace with your values
  instance_name = "HomeWork6"  # Replace with your values
}

#CREATE apache.sh

#!/bin/bash

sudo apt update
sudo apt install apache2 -y
sudo systemctl start apache2
sudo systemctl enable apache2


```