# BitSwan Platform

BitSwan is a platform for building automations and microservices directly in Jupyter Notebooks, and deploying them with a single click.  

## Key Use Cases
- **Automation of processes**  
- **Batch / real-time processing of data**  
- **Simple web applications**  
- **REST APIs**  


## Automation Server

The **Automation Server** is the runtime environment where BitSwan automations and microservices are deployed and executed.  

- Runs on a **Linux machine** with Docker or inside a **Kubernetes namespace**  
- Can host **multiple workspaces**, providing isolation between projects and teams  
- Operates in two modes:  
  - **Standalone** – fully functional for development and deployment of automations  
  - **Connected to AOC** – integrates with the Automation Operation Center (AOC) for advanced monitoring, process specification, and management features  

Even when not connected to the AOC, the Automation Server runs 100% autonomously.  


## Workspace / Runspace

A **Workspace** (or Runspace) is the logical separation unit within BitSwan, designed to isolate automations, users, and resources.  

Each workspace includes:  
- **GitOps** – for managing running automations:  
  - Deploy, restart, pause, or delete automations  
  - Access and monitor logs  
- **BitSwan Editor** – a customized VS Code server with the BitSwan extension:  
  - Develop and test automations/microservices using the BitSwan Python library and Jupyter  
  - Deploy automations with a single click  

### User Management
- Workspaces are the central building block of user access management  
- Users gain access either directly or through groups  
- Workspace membership determines visibility, management, and development permissions for automations

## Automation Operation Center (AOC)

The **AOC** is a modern web application that provides centralized visibility and management of BitSwan deployments.  

- Define and specify **processes**  
- Manage and monitor **automations**  
- Administer **automation servers** and **workspaces**  
- Control **user access and roles**  

When connected, Automation Servers and their workspaces continuously send information about deployed automations to the AOC.  

![AOC](/assets/bitswan-aoc.png)

## BitSwan Library

The **BitSwan Python library** is the foundation for building automations and microservices.  

- Includes reusable and configurable components for common integrations such as:  
  - Apache Kafka  
  - Elasticsearch  
  - Webhooks  
  - … (extendable with custom components)  
- Provides the **BitSwan compiler** that transforms Jupyter Notebooks into production-ready Python code

## How to Start

BitSwan supports several deployment models to fit different infrastructure needs.

- **Full Cloud**  
   - Both AOC and Automation Server are fully managed by us
- **Hybrid**  
   - AOC is managed by us, while the Automation Server runs in your infrastructure  
- **On-Premise**  
   - Both AOC and Automation Servers run entirely in your infrastructure

![BitSwan Deployments](/assets/bitswan-deployments.png)

### First Steps
Set up your environment using the [**BitSwan Automation Server CLI**](https://github.com/bitswan-space/bitswan-automation-server)

## Repositories

- [**bitswan (open source)**](https://github.com/bitswan-space/bitswan) – Python library for developing automations and microservices in Jupyter  
- [**bitswan-automation-server (open source)**](https://github.com/bitswan-space/bitswan-automation-server) – Orchestration system for running Automation Servers and managing workspaces/runspaces  
- [**bitswan-editor (mostly open source)**](https://github.com/bitswan-space/bitswan-editor) – Customized VS Code server tailored for BitSwan development and automation management  
- [**bitswan-gitops (open source)**](https://github.com/bitswan-space/bitswan-gitops) – GitOps-based orchestration system for deploying and managing automations inside workspaces  
- [**automation-operation-center (proprietary)**](https://github.com/bitswan-space/automation-operation-center) – Web application for process specification, monitoring, and management of BitSwan deployments  
