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
