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
7. **Documentation and Support:** Comprehensive setup and management guides.
8. **Community Engagement:** Foster user feedback and contributions.

## 6. Build a Custom OAuth 2.0 Authorization Server
- **Details**: Create an OAuth 2.0 server to handle secure token issuance, client registration, and access control. Supports standard flows like authorization code and token refresh.
- **References**: [List of Extensions](https://gist.github.com/joelonsql/e5aa27f8cc9bd22b8999b7de8aee9d47), [Tutorial](https://www.percona.com/blog/writing-postgresql-extensions-is-fun-c-language/), [Postgres docs for extension](https://www.postgresql.org/docs/current/sql-createextension.html).

- Got it! Here’s an updated project idea focused on building a custom OAuth server:

---

## 6. Build Your Own OAuth 2.0 Authorization Server

- **Abstract**: The goal of this project is to develop a standalone OAuth 2.0 authorization server that supports multiple applications, secure token handling, and offers fine-grained access control. Building an OAuth server from scratch allows greater flexibility and control over authentication and authorization flows, making it easier to create custom login solutions (e.g., "Sign in with our service") or integrate with proprietary authentication systems.

- **References**:
    - [RFC 6749: The OAuth 2.0 Authorization Framework](https://tools.ietf.org/html/rfc6749)
    - [Auth0's Guide to OAuth 2.0](https://auth0.com/docs/protocols/protocol-oauth2)
    - [Curity’s OAuth Server Documentation](https://curity.io/resources/learn/)
