# Project Description
To demonstrate the provisionin of Azure Storage Account for different subscription as a service catalog item from HPE Morpheus Enterprise.

# Technlogy Stack
* GitHub
* Terraform Templates
* HPE Morpheus Enterprise

# High Level Steps to Set-Up Infra
* Create and upload the repository with all the terraform templates.
* Use Morpheus variable wherever you want to get the input from the service catalog item. For example: <%= customOptions.azLocation %>
* Integrate the GitHub with HPE Morpheus Enterprise using the access token and not the password.
* Create Spec Templates in HPE Morpheus Enterprise.
    * Create spec templates for each .tf files.
    * Associate the .tf file after you select the source as Repository.
* Create an Instance Layout
* Create an Instance and assoicate the Layout created in above step
* Create Cypher in HPE Morpheus Enterprise if required for Azure crendentials.
* Create a Input & Option list.
* Create a Service Catalog item using the inputs and option list created in above step.

# Issues & Resolution To Set-Up Infra
* Not able to integrate GitHub with HPE Morpheus Enterprise with GitHub User/Password
    * [Resolution]: Generate access token in Settings in your github account and punch in while creating integration.

# Copyright(s)
2025 Hewlett Packard Enterprise Development LP