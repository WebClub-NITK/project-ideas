# WebClub Project Ideas

## Table of Contents

1. [Systems & Security SIG Ideas](#systems-&-security-sig-ideas)
2. [GDG Project Ideas](#gdg-project-ideas)

## Systems & Security SIG Ideas

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

### 1. Orbis
- **Project Idea**: Orbis is a comprehensive **open-source** event management platform, designed to streamline the experience of organizing, hosting, and participating in events. Originally intended for NITK, Orbis can be adapted for broader institutional and community use as an open-source solution.
  - **Core Features**:
    - **Event Listings**: Display events categorized by type (e.g., tech, non-tech).
    - **Social Sharing**: Simplified sharing of event details on social platforms.
    - **Registration & Application**: Manage participant registration with admin approvals.
    - **Notifications**: Automated email notifications for registration status updates.
    - **Project Submission**: Enable project submissions with links to videos, GitHub repositories, and README files.
    - **Team Management**: Support for team creation and management.
    - **Live Updates**: Real-time event updates for participants.
    - **Analytics Dashboard**: Visualize event data and attendance statistics.
    - **Feedback Collection**: Collect event feedback from participants.
    - **Networking Tools**: In-app chat and networking spaces to connect participants.
  - **Tech Stack/Skills Required/What you'll learn**:
    - Frontend: React/Next.js, responsive UI/UX design, CSS frameworks (TailwindCSS)
    - Backend: Node.js, Express, REST APIs, database management (PostgreSQL/MongoDB)
    - DevOps: Docker for deployment, basic CI/CD knowledge
    - Extras: Firebase/Supabase or similar for notifications, basic data visualization (for analytics dashboard)

### 2. Aegis (GDG x Systems)
- **Project Idea**: Aegis is an open-source platform for hosting Capture The Flag (CTF) competitions, designed to simplify event management and enhance user experience. Built with Django for backend robustness and Next.js for a responsive frontend, Aegis features Docker orchestration to dynamically handle challenge environments. This enables event organizers to manage Docker instances directly from the web interface, providing a scalable, customizable solution that can be deployed locally or on the cloud with ease.
  
  - **Core Features**:
    - **Docker-Orchestrated Challenges**: Each challenge is isolated in a dedicated Docker container, with automated management to start and stop containers based on participant actions, ensuring a secure, reproducible, and efficient environment.
    - **Customizable and Open-Source**: Allows customization of CTF rules, point systems, and themes. Built with modularity to support plugins and community-driven enhancements.
    - **User and Team Management**: Provides secure authentication with OAuth and JWT, supports team-based participation, and role-based access control for organized user permissions.
    - **Web-Based Admin Interface**: A Next.js-based admin dashboard for real-time monitoring, container management, and detailed analytics.
    - **Portable and Scalable Deployment**: Dockerized for flexible deployment, supporting local or cloud setups, ideal for both small-scale and large online competitions.

  - **Tech Stack/Skills Required/What you'll learn**:
    - Frontend: Next.js for building dynamic, responsive UIs, CSS frameworks for design
    - Backend: Django for robust data handling and Docker orchestration, API development
    - Database: PostgreSQL or MySQL for managing user, team, and event data
    - Docker: Docker Compose/Swarm for container management, resource allocation controls
    - Authentication: OAuth and JWT for secure access, user management

### 3. Photography Club Website
- **Project Idea**: Develop a modern website for the photography club with a static, visually engaging layout that highlights member portfolios, events, and club updates.
  - **Core Features**:
    - **Portfolio Showcase**: Display member portfolios and featured projects.
    - **Event Listings**: Announce upcoming events and photo walks.
    - **Blog Section**: Share tips, photography guides, and club news.
    - **Responsive Design**: Ensure the site is mobile-friendly and accessible.
  - **Tech Stack/Skills Required/What you'll learn**:
    - Frontend: Next.js/React, Tailwind CSS, Shadcn, Aceternity UI, Magic UI etc
    - Design: Basic UI/UX principles, familiarity with Figma or Adobe XD for creating mockups (optional, but good to have)
    - Extras: SEO optimization, basic image optimization techniques (for faster loading)

### 4. WebClub Website Team
- **Project Idea**: Build and maintain WebClub’s website, adding new features, improving UI, and implementing efficient backend solutions.
  - **Core Features**:
    - **Modular Development**: Introduce and maintain new website modules as needed.
    - **Authentication System**: Update and secure user login and authentication flows.
    - **UI/UX Enhancements**: Continuously improve the website’s user experience.
    - **Performance Optimization**: Regular maintenance for performance and load management.

### 5. HackClub Starter Kit (npx create-hc-app@latest)
- **Project Idea**: An open-source hackathon starter kit designed to support various tech stacks, including dApps, AI-based applications, and standard web apps. The kit includes built-in components and template options to simplify hackathon setup and usage.
  - **Core Features**:
    - **Multi-tech Stack Compatibility**: Support for dApps, AI, and web applications.
    - **Built-in Authentication**: Pre-configured authentication options.
    - **Component Library**: Reusable components for faster development.
    - **Template Options**: Choose from various project templates to jumpstart hackathon projects.
  - ***Tech Stack/Skills Required/What you'll learn**:
    - Frontend: React/Nextjs, CSS frameworks, component-based development
    - Backend: Node.js, Express, authentication protocols (OAuth, JWT)
    - Blockchain (optional): Solidity or similar for dApps, Web3.js or ethers.js for Ethereum integration
    - AI/Machine Learning (optional): Basic knowledge of integrating ML models if AI features are desired
    - Extras: Git for version control, familiarity with setting up hackathon-ready templates

### 6. Huntly (Maintenance & Improvement)

- **Project Idea**: Huntly is a cross-platform mobile application that facilitates real-world treasure hunts, encouraging participants to explore their surroundings and build connections. **This application is already built, but we need people to maintain, improve, and adapt it for college-wide use at meetups and events**. Huntly organizes treasure hunts with rewards, themed clues, and team-building elements powered by machine learning. The app offers both preset and customizable clues, unlocked via QR code scanning or verified through location tracking, with memory threads for users to share photos of their experiences.

  - **Core Features**:
    - **User Authentication and Profile Builder**: Users sign in with Google OAuth, set up profiles, and join or create hunts.
    - **Search and Organize Hunts**: Users can search for available hunts or organize their own using preset or custom clues.
    - **Clue Verification**: Features QR code scanning and location tracking for clue verification.
    - **Team Formation**: Uses K-Means clustering to match users with like-minded teammates for a collaborative experience.
    - **Leaderboard and Rewards**: Tracks and ranks team progress with rewards for top teams.
    - **Memory Threads**: Allows users to capture photos with teammates, creating a shared digital memory of the event.
  
  - **Skills Required**:
    - **Frontend**: **Flutter** for cross-platform mobile development on **Android/iOS**
    - **Backend**: Django Rest Framework and Flask for API development, including reward and memory management
    - **Packages**: Geolocator for location tracking, QR Code Scanner, Swagger for API documentation
    - **Machine Learning**: nltk and sklearn for team clustering algorithms
    - **Design**: Figma for app wireframing and prototyping
    - **Version Control**: Git/GitHub for collaboration and code management
   
  - **Github Repo** - https://github.com/Team-Huntly/Huntly
    
   
    





