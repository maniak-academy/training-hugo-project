---
weight: 10
title: "Setup"
description: ""
icon: "article"
date: "2023-12-22T14:06:28-05:00"
lastmod: "2023-12-22T14:06:28-05:00"
draft: false
toc: true
---


## Setup the AWS Environment

The first step is to configure your AWS KEY and Secret so that we can build the infrastructure. Log into your AWS console and generate a key/secret-id. Execute the command below and paste your information.

```
aws configure
```

## Deploy the Infrastructure

The next step is to deploy the infrastructure, so let's clone the repo and get into the specific folder.

```
git clone https://github.com/maniak-academy/aws-lab-getting-started-with-Ansible-Fortigate.git

cd aws-lab-getting-started-with-Ansible-Fortigate/terraform
```

Next, let's initate terraform and apply the deployment. The output will give all the information needed to access the Fortigate Firewall. It takes about 5-8 mintues to deploy

```
terraform init

terraform apply
```



...