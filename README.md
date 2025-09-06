# PROVISIONING-DOCKER-INFRASTRUCTURE-USING-TERRAFORM

<img width="312" height="156" alt="Terraform logo" src="https://github.com/user-attachments/assets/6c0d421f-24f8-43b2-9f9c-1886150415e2" />


###OVERVIEW OF PROJECT
Creating and managing Docker infrastructure using Terraform involves defining your desired Docker resources in Terraform configuration files and then using Terraform commands to provision and manage those resources.

#PREREQUISITES
Install Prerequisites:
1. Terraform: Install the Terraform CLI on your system.
2. Docker: Install Docker Desktop (or Docker Engine) on your system.

1. The file includes terraform block which defines the provider and the terraform versions
   
 <img width="468" height="169" alt="image" src="https://github.com/user-attachments/assets/0d7bd693-2081-4dab-a629-d731807abf2d" />


3.  Main.tf file containing infrastrucutre for docker infrastucture
   
 <img width="468" height="218" alt="image" src="https://github.com/user-attachments/assets/5c3b76e7-9373-4ad6-a873-486846242f1e" />

4. Terraform fmt - 
We recommend using consistent formatting to ensure readability. The terraform fmt command automatically reformats all configuration files in the current directory according to HashiCorp's recommended style.
<img width="321" height="32" alt="image" src="https://github.com/user-attachments/assets/7ee65ffa-21f8-450d-95a4-13f81ca92e72" />

5.Validate configuration
we make sure our configuration is syntactically valid and internally consistent by using the terraform  validate command

<img width="303" height="29" alt="image" src="https://github.com/user-attachments/assets/853c33b5-24c9-4ffe-b8e3-911f1121e73c" />

6. Project is initialized which downloads the plugins that allows terraform to interact with docker, this is done by running terraform init

<img width="468" height="242" alt="image" src="https://github.com/user-attachments/assets/3fd96314-76ce-432c-a35f-a1b0459379eb" />

7. Provision the NGINX server container with apply. When Terraform ask you to confirm type yes and press enter.
   
<img width="468" height="261" alt="image" src="https://github.com/user-attachments/assets/9e63dd01-1e1a-46f3-9258-eae046eafcda" />

8. We can run docker ps to view how newly created infrastructure

   <img width="412" height="275" alt="image" src="https://github.com/user-attachments/assets/43b7e218-e888-4998-bbaa-76dc8971f42f" />

   


