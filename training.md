# DevOps Bootcamp
This bootcamp should span between 3 ~ 5 days depending on the knowledge/competence of the candidate.

## Day 1
Spend no more than 1 hour with the candidate.

### Introduction
Talk about the below topics. Try and restrict the conversation to below 30 minutes. You do not want to overload the candidate with information.
- Junior: After the conversation, ask the candidate to start learning Docker.
- Senior: After the conversation, ask the canddiate to start going through the _DMS_ project.

#### Overall Architecture
Talk about the **2 categories** of software applications that we have at VAT IT. _Core application suite_ and _peripheral supporting applications_. Talk about the 2 different underlying infrastructures that the 2 categories of applications operate on.

##### Core Application Suite (aka _Dragon Services_)
**Dragon** and associated services make up the fundamental software that VAT IT operates on. Together, the entire system can be thought of as a _custom accounting software_. To dive into the details of the various components follow [The Hitchhiker's Guide to Vat IT](https://vat-it.atlassian.net/wiki/x/qPQoAw).

##### Peripheral Supporting Applications
There are numerous applications/services that support the _Core Application Suite_. These include various partner integrations, automation, data science etc.

##### 1st infrastructure type: Windows Virtual Machines (Ansible)
Legacy applications are run this way. In the process of deprecating functions.

##### 2nd infrastructure type: Docker and Kubernetes
Newer applications (**all** new applications going forward) are run this way. **Cloud Native** and **Docker** first. Applications that either use **serverless** or **Kubernetes**.

#### Developer Responsibility
There are 2 mantras that the developer need to always keep in mind:
- Follow good DevOps practices
- Transparency of source code

##### Good DevOps Practices
Check the DevOps Documentation.

##### Source Code Transparency
This mainly refers to the documentation of the code (others need to **know** what this application does), maintainability of the code (others need to **understand** nuances associated with this application) and longivity ofg the code (others need to be **able** to take over your application even after your leave).

This basically leads to the conversation of **good documentation** and **good tests**.

#### Deployment Pipeline
Talk about the Docker -> Jenkins -> Kubernetes pipeline. Talk about what happens at each stage, docker to package the application, Jenkins for CI/CD, Kubernetes for deployment of applications.

#### Development Workflow / Project structure
Talk about the 3 files that are in the root directory of every project (2nd infrastructure type): _Dockerfile_, _Jenkinsfile_ and _Kubernetes deployment.yml_.

## Day 2
Spend no more than 1.5 hours with the candidate.

#### Docker
Start going through **Docker** with the candidate, check the progress of the candidate in terms of the understanding of Docker. Ask them to complete the _vote_ lab in the devops-bootcamp [repository](https://bitbucket.org/vatit-admin/devops-bootcamp/src/master/).

Set a time with the candidate to go through the task.

## Day 3
Spend no more than 1 hour with the candidate.

#### Jenkins
Ask the candidate to complete the _blog_ lab in the devops-bootcamp [repository](https://bitbucket.org/vatit-admin/devops-bootcamp/src/master/). Go through what is required from them. All they need to do is to add a _Jenkinsfile_ to the repository, there is no need to make changes to the source code.

## Day 4
Spend no more than 1 hour with the candidate.

### Kubernetes
Explain the basic concepts of Kubernetes (concepts of the cluster, nodes, pods, containers, deployments, services, namespaces). Ask them to watch [What is Kubernetes?](https://www.youtube.com/watch?v=R-3dfURb2hA). Go through the deployment.yml file with them.
