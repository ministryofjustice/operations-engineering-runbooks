---
owner_slack: "#operations-engineering-alerts"
title: Ways of Engineering
last_reviewed_on: 2024-11-12
review_in: 3 months
---

# Ways of Engineering

This foundational document outlines our collective approach to engineering practices, fostering a culture of continuous improvement, innovation, and excellence. It is a compass for our technical journey, guiding us to make informed decisions, embrace best practices, and explore new technological frontiers. This document aims to harmonise our engineering efforts, ensuring efficiency, quality, and sustainability in our projects.

**Statuses:**

- ✅ Accepted
- 🧪 Experimenting
- 💡 New idea (waiting to be discussed by the team)

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
