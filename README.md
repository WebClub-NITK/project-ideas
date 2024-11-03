# Systems Project Ideas
This repository is for maintaining project ideas for the Systems and Security SIG.

---

## 1. Create a PostgreSQL Database Extension
- **Details**: Creating an extension for PostgreSQL can be done in C. The usefulness of the extension depends on the problem it aims to solve. For example, we could build an extension that displays the query plan of the SQL engine. Open to additional suggestions for potential functionalities.
- **References**: [List of Extensions](https://gist.github.com/joelonsql/e5aa27f8cc9bd22b8999b7de8aee9d47), [Tutorial](https://www.percona.com/blog/writing-postgresql-extensions-is-fun-c-language/), [Postgres docs for extension](https://www.postgresql.org/docs/current/sql-createextension.html).

## 2. Idea: Build a Serverless Function-as-a-Service (FaaS) Application
- **Details**: Develop a lightweight serverless Function-as-a-Service platform that allows users to deploy and manage isolated functions in response to events. The platform should support multiple languages (e.g., Python, Node.js) and offer features like auto-scaling, event-driven triggers, and simple API integration. Additional functionalities can include a dashboard for monitoring function performance, error logs, and usage metrics.
  
  - **Core Features**:
    - **Multi-language support**: Enable users to deploy functions in various programming languages.
    - **Event-driven triggers**: Integrate with popular services (like HTTP endpoints or message queues) to trigger functions.
    - **Auto-scaling**: Dynamically scale up/down based on workload demands.
    - **Monitoring and logging**: Provide real-time logs, usage metrics, and error tracking for deployed functions.

- **References**: 
  - [AWS Lambda Documentation](https://docs.aws.amazon.com/lambda/latest/dg/welcome.html)
  - [Serverless Framework](https://www.serverless.com/)

## 3. P2P File Sharing Tool in Golang
- **Abstract** - The idea is to build a tool that allows people to share large files directly without having to load them on a third party storage service first. Although there are already a lot of such tools, we are hoping to use Golang's extensive support for concurrency to make it easier and faster to share multiple files and folders at the same time and with multiple recievers.  

- **Features**
  - Sharing files and folders directly between users
  - A clean and intuitive CLI tool for a good user experience.
  - Share files concurrency to a single or multiple recievers.
  - Ability to open up a temporary data server and allow clients to pick whichever files they want.
  - Support file compression.
  - Ability to generate one time share links (once a reciever uses the link its expired)
  - Allow users to resume pending transfers.
  - Provide E2E encryption to the users.

- **References**
  - [fs-cli](https://github.com/spectre10/fs-cli)
  - [pion/webrtc](https://github.com/pion/webrtc)
  - [gfile](https://github.com/Antonito/gfile)

## 4. Open Source Mentorship
- **Abstract** - Instead of a project, we can have an open source mentorship program spanning over 2-3 months where seniors guide the juniors on how to get started with contributing to the Linux kernel or other major open source systems projects. Eventually, this might significantly increase the number of selections from Systems SIG (and wec) in GSoC and LFX.

- **Features**
    - Regular meets between seniors and juniors (for guidance and tracking progress)
    - Make solid open source contributions to the linux kernel or any other major open source project
  


## 5. Docker Host Integration Tool

## Overview

This tool aims to integrate Docker hosts across different machines, even those not on the same network, using VPN technology for seamless communication.

## Objective

Create a unified network for Docker hosts, allowing all containers to communicate as if on the same local network, accessible from a single VPS or designated machine.

## Key Features

1. **VPN Integration:** Secure connections between Docker hosts.
2. **Centralized Access:** Unified access point for all containers.
3. **Scalability:** Easy addition of new Docker hosts.
4. **User-Friendly Interface:** Simplified management and monitoring.
5. **Monitoring and Logging:** Track performance and activity.
6. **Security Features:** Robust data protection.

## 6. Build Your Own OAuth 2.0 Authorization Server

- **Abstract**: The goal of this project is to develop a standalone OAuth 2.0 authorization server that supports multiple applications, secure token handling, and offers fine-grained access control. Building an OAuth server from scratch allows greater flexibility and control over authentication and authorization flows, making it easier to create custom login solutions (e.g., "Sign in with our service") or integrate with proprietary authentication systems.

- **References**:
    - [RFC 6749: The OAuth 2.0 Authorization Framework](https://tools.ietf.org/html/rfc6749)
    - [Auth0's Guide to OAuth 2.0](https://auth0.com/docs/protocols/protocol-oauth2)
    - [Curity’s OAuth Server Documentation](https://curity.io/resources/learn/)

## 7. eBPF-Based File Integrity Monitoring

- **Abstract**: Argus is a file integrity monitoring tool designed to provide real-time monitoring of file system changes using eBPF (extended Berkeley Packet Filter). Leveraging the power and efficiency of eBPF, Argus offers a lightweight and highly performant solution for detecting and responding to unauthorized modifications, helping ensure the integrity and security of critical files and directories. Argus focuses on low-latency monitoring, enabling quick detection and response for security-critical environments.

- **References**:
    - [Introduction to eBPF](https://ebpf.io/what-is-ebpf/)
    - [eBPF Program Types Documentation](https://docs.cilium.io/en/stable/bpf/)
    - [File Integrity Monitoring](https://www.varonis.com/blog/file-integrity-monitoring)


# GDG Project Ideas

## Orbis
- **Project Idea**: Orbis is a sophisticated event management platform designed to simplify and elevate the experience of organizing, hosting, and participating in events. Originally envisioned for NITK, Orbis is a versatile, open-source solution for institutions, communities, and individuals aiming to streamline event coordination.
- **Features**: Event Listings, Event Types (tech, non-tech, etc.), Social Sharing, Registration & Application, Admin Approval for Applications, Email Notifications (acceptance/rejection), Project Submission (video, README, GitHub, links), Team Management, Live Updates, Analytics Dashboard, Feedback Collection, Networking Tools (in-app chat, networking spaces).
- **Organizing SIG**: GDG
- **Status**: Not Started
- **Priority**: High
- **Main Lead**: Mardav
- **Secondary Lead**: Rohith V
- **Project Members**: 
- **Start Date**: 10/26/2024
- **End Date**: 10/26/2024
- **Strategy**: 
- **Key Milestones**: 
- **Stack & Dependencies**: 

---

## Aegis
- **Project Idea**: Aegis is an open-source platform for hosting Capture The Flag (CTF) competitions, designed to simplify event management and enhance user experience. Built with Django for backend robustness and Next.js for a responsive frontend, Aegis features Docker orchestration to dynamically handle challenge environments.
- **Features**: TBD
- **Organizing SIG**: GDG, Systems
- **Status**: Not Started
- **Priority**: High
- **Main Lead**: Apoorva
- **Secondary Lead**: Mardav
- **Project Members**: 
- **Start Date**: 10/26/2024
- **End Date**: 10/26/2024
- **Strategy**: 
- **Key Milestones**: 
- **Stack & Dependencies**: Django, Next.js, Docker

---

## Photography Club Website
- **Project Idea**: Build the photography club website from scratch (static webpage).
- **Features**: 
- **Organizing SIG**: GDG
- **Status**: Not Started
- **Priority**: High
- **Main Lead**: Hariharan
- **Secondary Lead**: Utkarsh
- **Project Members**: 
- **Start Date**: 10/26/2024
- **End Date**: 10/26/2024
- **Strategy**: 
- **Key Milestones**: 
- **Stack & Dependencies**: 

---

## HESC Conference Website
- **Project Idea**: 
- **Features**: 
- **Organizing SIG**: GDG
- **Status**: Completed
- **Priority**: High
- **Main Lead**: Hariharan
- **Secondary Lead**: Utkarsh
- **Project Members**: Suyash, Mardav, Utkarsh
- **Start Date**: 10/30/2024
- **End Date**: 11/15/2024
- **Strategy**: 
- **Key Milestones**: 
- **Stack & Dependencies**: 

---

## WebClub Website Team
- **Project Idea**: Building new modules, maintaining the website, UI improvements, authentication.
- **Features**: 
- **Organizing SIG**: GDG
- **Status**: In Progress
- **Priority**: Medium
- **Main Lead**: Hariharan
- **Secondary Lead**: Apoorva
- **Project Members**: Hariharan, Mardav, Apoorva, Aahil, Utkarsh, Fahim, Shubham
- **Start Date**: 
- **End Date**: 
- **Strategy**: 
- **Key Milestones**: 
- **Stack & Dependencies**: 

---

## HackClub Starter Kit (npx create-hc-app@latest)
- **Project Idea**: Open-source hackathon starter kit with support for various tech stacks, including dapps, AI-based apps, and simple web apps. Features built-in authentication, layouts, components, and template options.
- **Features**: 
- **Organizing SIG**: GDG
- **Status**: Not Started
- **Priority**: Medium
- **Main Lead**: Shubham
- **Secondary Lead**: 
- **Project Members**: 
- **Start Date**: 
- **End Date**: 
- **Strategy**: 
- **Key Milestones**: 
- **Stack & Dependencies**: 

---



