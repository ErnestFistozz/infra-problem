# Infrastructure provisioning

The proposed tool for provisioning infrastructure is `Terraform`
The structure would look something like this:
- Infrastructure
    - Template
        - Dev
        - End-to-End
        - Staging/(Quality Assurance)
        - Production
There would be a generalised template for provisioning machines in the cloud the
and then there would be a module which would allow developers to supply corresponding machine requirements.

# Deploying microservices in the cloud
The best-way to go about microservices is to utilise kubernetes. the application is already split into respective parts. What need to be done these need to be pushed  as images separately into the respective container registery of the chosen provider. Depending on the cloud provider, either AKS, or EKS or GKE cluster will be provisioned and the respective kubernetes resources would be deployed on the images created. 

# implementing CI/CD
This also goes back to the cloud provider chose, if its Azure then Azure devops would be utilised and if its AWS, then AWS corresponding DevOps service would be utilised.

