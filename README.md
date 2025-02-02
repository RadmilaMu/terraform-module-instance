# terraform-module-instance

```hcl
module "instance" {
  source  = "RadmilaMu/instance./module"
  version = "1.0.0"
  region = "us-east-2"   # Replace with your values
  instance_type = "t2.micro"  # Replace with your values
  instance_name = "HomeWork6"  # Replace with your values
}

#CREATE apache.file

#!/bin/bash

sudo yum install httpd -y
echo "Hello, World!" | sudo tee /var/www/html/index.html > /dev/null
sudo systemctl start httpd
sudo systemctl enable httpd


```