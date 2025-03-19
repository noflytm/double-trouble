# Lab Overview: Deploying a Custom Nginx Server with Terraform

In this lab, your goal is to deploy a custom Nginx server on a dedicated server using Terraform. You have been provided with a Terraform configuration intended to automate this deployment. However, the configuration contains several issues that prevent successful execution.

Your task is to identify and fix these issues, ensuring that Terraform correctly provisions the server, installs Nginx, and serves a custom `index.html` page. By completing this lab, you will gain hands-on experience in debugging Terraform configurations and deploying infrastructure efficiently.


## Deployment diagram

![](./img/tbs1.png)

 
## Solution Breakdown

### Infrastructure configuration will include:

 - VPC & Networking – Setting up the necessary networking components such as subnets, route tables, and internet access.
 - Security Groups – Configuring firewall rules to allow necessary traffic (e.g., HTTP/HTTPS).
 - Compute Instance – Launching a dedicated server to run the Nginx service.
 - S3 Bucket – If required, managing storage for static files or logs.

### Rules & Constraints:

- Fix errors in the provided Terraform configuration to ensure a successful deployment.
- Do not remove existing resources, but you may modify or add them if necessary.
- Add new resources only if required for a proper deployment.
- All changes must be committed to a fork repository.


## Task

Your objective is to fix any errors preventing the Terraform configuration from being successfully applied.

Key Steps:

- Carefully review all resource parameters.
- Refer to the Terraform documentation on [provisioners](https://developer.hashicorp.com/terraform/language/resources/provisioners/syntax), particularly the section on [creation-time provisioners](https://developer.hashicorp.com/terraform/language/resources/provisioners/syntax#creation-time-provisioners).
- Modify the index.html file to include your name in the message, using the Terraform variable student_name:
```Example output:
  Greetings from John Doe! This is a Terraform task.
```

## Definition of Done:

- The Terraform configuration applies without errors.
- No resources deleted from Terraform configuration(but they might be changed).
- The Nginx server is accessible via its public IP.
- The custom page displays the correct message, including your name.

That's it — once these conditions are met, you've successfully completed the lab!

