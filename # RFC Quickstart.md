# RFC Quick Start

## :point_up: Goal
The QuickStart feature comes with the proposal to facilitate a quick start in the provisioning of complex stacks and most common to CloudController users.
We offer the user a fully assisted first version where he will inform us of the desired configurations for the desired resource group to be provisioned,
and we build your first flow creating your feature/branch from the first PR to the time eligible for deployment, without need to write a single line of HCL code.
Available in their account, be it AWS or GCP.

## Motivation
Offer greater flexibility, less bureaucracy and ease to understanding and adoption of lay or advanced users to the IaC provisioning flow through CloudController, 
so that it can guarantee complex resources such as EKS, EMR, ECS and others, in a more peaceful way for a first contact with the technologies of the moment.

## Cases proposal
- Allows users who have never worked with Cloud or Terraform and need to manage their resources through CloudController;
- Facility for those who need to quickly start building a simple or complex stack without having to write HCL code for it;
- New stacks faster;
- Understand the adoption process for creating a stack in cloudcontroller;
- Provision complex resources with terraform without prior contact;
- Agility in delivering value;

## 💡 Mental Map:

![POC_CC_QUICKSTART](https://raw.githubusercontent.com/meli-gkato/rfc-images/main/POC_CC_QUICKSTART.0.1.0.drawio.png)

## At the time of stack creation
The user will be able to select one or more resource groups to provision. 
The initial idea is to offer a form of computational and strategic definitions for the provisioning of infrastructure as code (IaC). 
In the following example, we will show a form template for adopting an EKS cluster in the AWS provider.

### Use Case - EKS Service Form

![use_case_EKS_service_form](https://raw.githubusercontent.com/meli-gkato/rfc-images/main/use_case_EKS_service_form.png)

### Page Resources AWS EKS Form

Example of page where you can view, for AWS accounts, the icons of types of services available for the first version. 
Once the user makes the choose, then a form will appear for you to fill in with the user's needs in relation to the service 
in the application. In our example, in Quick Start tab, the resource/service chosen is an EKS.

![quickstart_eks_form_view](https://raw.githubusercontent.com/meli-gkato/rfc-images/main/quickstart_eks_form_view.png)

### Status creating stack version

Sample page where you can view step by step when your version is still being created.

![cms_executions](https://raw.githubusercontent.com/meli-gkato/rfc-images/main/quickstart_eks_modal_creating.png)

### Nice to Have

#### [Argo CD](https://argo-cd.readthedocs.io/en/stable/):

Application definitions, configurations, and environments should be declarative and version controlled. Application deployment and lifecycle management should be automated, auditable, and easy to understand.

#### [OpenID Connect (OIDC)](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_roles_providers_create_oidc.html)

[Introducing OIDC](https://aws.amazon.com/pt/blogs/containers/introducing-oidc-identity-provider-authentication-amazon-eks/) - identity provider authentication for Amazon EKS

IAM OIDC Identity Providers are entities in IAM that describe an external identity provider (IdP) service that supports the OpenID Connect (OIDC) standard. You use an IAM OIDC Identity Provider when you want to establish trust between an OIDC-compliant IdP and your AWS account. This is useful when you are building a mobile app or web app that needs to access AWS resources but don't want to create a shortcode custom or manage your own user identities.


## Stakeholders
@mguelar 
@leacevedo 
@meli-diteixeira 
@meli-gkato
@arthur-meli


