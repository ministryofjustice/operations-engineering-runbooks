---
owner_slack: "#operations-engineering-alerts"
title: Ways of Engineering
last_reviewed_on: 2025-02-12
review_in: 3 months
---

# Ways of Engineering

This foundational document outlines our collective approach to engineering practices, fostering a culture of continuous improvement, innovation, and excellence. It is a compass for our technical journey, guiding us to make informed decisions, embrace best practices, and explore new technological frontiers. This document aims to harmonise our engineering efforts, ensuring efficiency, quality, and sustainability in our projects.

**Statuses:**

- ✅ Accepted
- 🧪 Experimenting
- 💡 New idea (waiting to be discussed by the team)

## Hosting Services and Infrastructure

### ✅ Use Cloud Platform as the Primary Hosting Platform

The Cloud Platform is made for hosting modern, containerised applications and provides easy access to most AWS services for infrastructure requirements.

We should host new applications and infrastructure on the Cloud Platform, unless there are specific reasons not to.

### ✅ Use Modernisation Platform as the Secondary Hosting Platform

The Modernisation Platform is made for hosting applications that are not yet containerised or where a project has complex infrastructure requirements.

We have chosen to only have one environment* in the Modernisation Platform. This environment is called [operations-engineering](https://github.com/ministryofjustice/modernisation-platform/blob/main/environments/operations-engineering.json). AWS Accounts in this environment should be used for all infrastructure deemed suitable to host in the Modernisation Platform.

Any production level services should be deployed into the `operations-engineering-production` AWS Account. This account can only be deployed to via code changes in [modernisation-platform-environments](https://github.com/ministryofjustice/modernisation-platform-environments)

> ***An environment in the Modernisation Platform can mean one of two things:**
>
> - **A namespace which encapsulates several AWS accounts i.e. `operations-engineering`**
> - **A traditional environment for deployment such as `development`, `production` etc. combined with the Namespace definition above, these create the names for the AWS Accounts created i.e `operations-engineering-development`, `operations-engineering-production` etc.**
>
> In the descriptions in this section, I have opted to use `environment` to describe the `namespace` and `AWS Account` to describe the `traditional environment` to avoid confusion.

#### Why Are We Only Using One Environment?

While the team gets more familiar with the Modernisation Platform, we have decided to only use one environment. This will help us to keep things simple and avoid confusion.

We will review this decision in the future when there is a need to add more environments.

#### Cloud Platform vs Modernisation Platform

|Cloud Platform|Modernisation Platform|
|:-----|:-----|
|Provides a namespace within the CP AWS account to contain your resources|Creates AWS accounts for each environment (dev, test, pre-prod, prod) under your namespace environment|
|Intended for microservices|Intended for services requiring more complex infrastructure|
|Access to some AWS resources restricted (eg no AWS Lambda)|Full control and full access to AWS tools|
|Provides access to CPs Kubernetes cluster|Provides Security baselines, Isolated networking, CI/CD for infrastructure|
|Example: Join GitHub app (🪦); containerised app hosting a website, running small supporting infra|Example: NOMIS; mainaining a huge database, restricting access, integrating with microservices (which may be on CP)|

### ✅ Do Not Use The MoJ Digital Services (DSD Account) to Host Services

The MoJ Digital Services AWS Account is a legacy account that is currently owned by several teams and is not suitable for hosting new services.

Existing services owned by our team hosted in the MoJ Digital Services AWS Account  should be migrated to the Cloud Platform or Modernisation Platform.

## **Package Management and Environment**

### ✅ Python as the Primary Programming Language

We have decided to continue using Python as our primary programming language due to the following reasons:

- Python has a large and active community, ensuring abundant resources, libraries, and support.
- Python's simplicity and readability make it easier to onboard new developers, especially those with an interest in infrastructure and DevOps.
- For our team's requirements, Python's flexibility and emphasis on rapid development suit our needs well. We prioritize the velocity of features over extreme performance or resilience.

### **✅ Use PipEnv for Python Package Manager**

We are experimenting with adopting PipEnv as our Python package manager, moving away from our current setup using Pip. PipEnv offers a more streamlined approach to managing package dependencies and Python environments. This tool combines the best aspects of various packaging tools into a single interface, aiming to improve our workflow and project consistency. The experiment will assess PipEnv's impact on our development process, focusing on ease of use, dependency resolution, and environment management.

## **Security and Dependency Management**

### **✅ Replace Dependabot with Trivy for CVE Dependency Management**

To enhance our security posture and streamline the management of vulnerabilities within our dependencies, we are experimenting with replacing Dependabot with Trivy. This shift aims to leverage Trivy's comprehensive vulnerability detection across multiple languages and package managers and ease of integration into our CI/CD pipelines. During this experimental phase, we will evaluate Trivy's effectiveness in identifying and mitigating known vulnerabilities, comparing it to Dependabot's performance and utility.

### **✅ Implement CodeQL for Python Code Security Review**

To uphold the highest security standards in our Python codebase, we have decided to integrate CodeQL into our development workflow. CodeQL will serve as a critical tool in identifying security weaknesses within our Python code at pull request (PR) stages and on a regular basis through automated scans. Including CodeQL aims to enhance our proactive security measures, allowing us to address vulnerabilities effectively and maintain the integrity of our applications.

## Adding/Adjusting Ways of Engineering

To maintain the relevance and effectiveness of our Ways of Engineering, we encourage team members to propose adjustments or additions. Suggestions can be discussed in dedicated Slack channels, Engineering Guild meetings, or directly through Pull Requests. Your contributions are crucial in ensuring our engineering practices remain dynamic, inclusive, and aligned with our goals.

### Experimental Engineering Practices

We're committed to innovation in our projects and how we work together as an engineering team. Experimenting with new practices allows us to improve and adapt to the changing tech landscape continuously. Participation and feedback from all team members are essential for these experiments to yield valuable insights and guide our evolution.
