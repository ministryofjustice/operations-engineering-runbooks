---
owner_slack: "#operations-engineering-alerts"
title: Agile Delivery
last_reviewed_on: 2024-07-08
review_in: 3 months
---

# Agile Delivery

A practical guide for Operations Engineering's Agile Delivery methodologies and practices.

The foundation of Operations Engineering's Agile Delivery is [Our Ways of Working](https://runbooks.operations-engineering.service.justice.gov.uk/documentation/internal/team/ways-of-working.html), which should be read before reading this guide.

Many ideas in this guide are based on the following resources, which can be used as a reference or for further reading:

- [GDS Agile Delivery](https://www.gov.uk/service-manual/agile-delivery)
- [Agile Manifesto](https://agilemanifesto.org/)
- [Agile Manifesto - Principles](https://agilemanifesto.org/principles.html)

## Introduction

Agile, by principle, rarely produces a _'one shoe fits all'_ solution for delivery and project management.

Operations Engineering has documented the teams' agreed approach below, enabling the process to be critically analysed and reflected upon later. This ensures continuos improvement to how projects are managed and services are delivered.

## Phases of Delivery

Detailed in the [GDS Agile Delivery](https://www.gov.uk/service-manual/agile-delivery) guidance, there are 5 phases of a project:

- Discovery
- Alpha
- Beta
- Live
- Retirement

In this section, there will be a small summary of each phase, quickly followed by the specific details of how Operations Engineering approach the phase in the life cycle.

For each phase, Operations Engineering will create a [GitHub Milestone within the operations-engineering repository](https://github.com/ministryofjustice/operations-engineering/milestones) to indicate the start of a new phase.

### Discovery

Detailed in [How the discovery phase works](https://www.gov.uk/service-manual/agile-delivery/how-the-discovery-phase-works), the discovery phase is all about understanding the problem.

#### Outcomes of Discovery

At the end of discovery, Operations Engineering will have understood, documented and agreed on the following:

- ✅ **Key Stakeholders** - these are the stakeholders that will gain the most from a solution in the identified problem space. Frameworks such as [Stakeholder Mapping](https://en.wikipedia.org/wiki/Stakeholder_analysis#Stakeholder_mapping) can help when deciding key stakeholders.
- ✅ **Key Stakeholder - Needs** - the needs of the stakeholders should be well understood. These will aid in scoping the problem down to provide a solution that resolves a whole problem for users.
- ✅ **Process Diagram** - process diagrams are helpful visual aids for simply explaining processes. Creating a process diagram by the end of discovery will help the team to identify problem areas, smaller scoped issues that could be tackled first, constraints, and help communication with stakeholders by using a common view.
- ✅ **Scope** - there will be an agreement on the scope of the problem the team will attempt to solve. Being able to scope the problem sufficiently will help ensure a successful solution can be delivered to stakeholders in a timely manner. _Don't attempt to solve the whole problem, but ensure you solve a whole problem for the user._
- ✅ **Problem Statement** - by the end of the discovery - the team is able to succinctly express the problem providing useful insight into the problem domain i.e. the users and their needs.
- ✅ **Success Metrics** - agreement of success metrics by the end of discovery will ensure the team focuses on solving the right problem and enable us to later critically evaluate solutions that are built.
- ✅ **Decision on Whether to Continue** - At the end of discovery, Operations Engineering will have enough information about the problem to decide whether it is valuable to do something about the problem.

**Primary Lifecycle Stages:** Planning, User Research, Data Gathering

### Alpha

Detailed in [How the alpha phase works](https://www.gov.uk/service-manual/agile-delivery/how-the-alpha-phase-works), the alpha phase is all about testing assumptions with users.

**Primary Lifecycle Stages:** Development, User Research, User Testing

### Beta

Detailed in [How the beta phase works](https://www.gov.uk/service-manual/agile-delivery/how-the-beta-phase-works), the beta phase is all about starting to solve the problems.

**Primary Lifecycle Stages:** Development, Deployment, User Testing

### Live

Detailed in [How the beta phase works](https://www.gov.uk/service-manual/agile-delivery/how-the-beta-phase-works), the live phase is all about supporting a service in a sustainable way.

**Primary Lifecycle Stages:** Maintenance, Monitoring

### Retirement

Detailed in [Retiring your service](https://www.gov.uk/service-manual/agile-delivery/retiring-your-service), the retirement phase is all about turning the service off.

**Primary Lifecycle Stages:** Monitoring, Decommissioning

## Types of Work

Loosely based on _The Four Types of Work (Phoenix Project)_

- Unplanned
- Tech Debt
- Experiment
- Project
  
## Lifecycle Stages

Loosely based on [The Systems Development Lifecycle](https://en.wikipedia.org/wiki/Systems_development_life_cycle) and the [Project Management - Project Lifecycle](https://en.wikipedia.org/wiki/Project_management#Project_lifecycle)

- Planning
- User Research
- Data Gathering
- Development
- Deployment
- User Testing
- Monitoring
- Maintenance
- Decommissioning
