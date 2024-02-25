# MediaWiki-Deployment-Automation

**Overview:**
This Terraform script automates the deployment of a MediaWiki instance on an AWS EC2 instance using Terraform and Ansible. It provisions the necessary infrastructure components such as VPC, subnets, security groups, and EC2 instance, and then configures the instance using Ansible to set up MediaWiki.

The Ansible playbook is executed on the localhost.
Tasks include updating and upgrading packages, installing required software packages like Apache, MySQL, PHP, and Ansible, creating directories, downloading and extracting MediaWiki tarball, configuring MySQL user and database, and configuring MediaWiki itself.
Additionally, it installs the php-intl extension and restarts the Apache server to ensure compatibility with MediaWiki.

This integrated approach automates the deployment and configuration of MediaWiki, streamlining the setup process for users. Users only need to execute the Terraform script to provision and configure the MediaWiki instance automatically.

**Steps To Use the Script**

1. Download the terraform file to your local machine
2. Install terraform
3. Change name and path to your .pem file
4. Run the terraform commands 
  - terraform init
  - terraform plan
  - terraform approve

Note: On running the terraform file it will automatically download and execute the ansible yml file to configure mediawiki app.
      If you want to clone and run the script then please change the wget path to your git repository.  