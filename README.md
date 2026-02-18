## In a hurry
Top 3 projects that showcases my learning:
1. **[LZStock](#full-stack-lzstock)** (This is the one you must check if you have to pick one) 
2. [Data Pipeline](#data-pipeline-us-stock-financial-report-dumper)
3. [Price Dashboard](#full-stack-price-dashboard)

## 📂 Portfolios
### Full-stack: [LZStock](https://lzstock.app)

LZStock is a stock screener that saves you time to help you make decisions quickly. 

#### LZStock Tech blog
- **[What and How I built?](https://blog.lzstock.app/blog/what-I-built)** (This is the only page you have to check if you have no time)  
- [Why do these topics matter?](https://blog.lzstock.app/blog/why-these-topics-matter)

#### [LZStock Labs & Open Source](https://github.com/LZStock-OS)
- [Service-guardian](https://github.com/LZStock-OS/service-guardian): a health check and service registration library written in GO

𝐖𝐡𝐚𝐭 𝐢𝐬 𝐭𝐡𝐢𝐬?   
- This is a self-initiated project built to demonstrate my comprehensive understanding of how to construct a fundamental, general-purpose, production-ready system.
- I chose an interesting topic: A US stock screener based on financial statements sourced from www.sec.gov.
- This project centers on developing a foundational framework, exploring best practices, and acquiring experience through genuine challenges.

𝐇𝐨𝐰 𝐢𝐬 𝐭𝐡𝐢𝐬 𝐩𝐫𝐨𝐣𝐞𝐜𝐭 𝐮𝐧𝐢𝐪𝐮𝐞?
- Encompassed the entire development lifecycle, from initial design through to final deployment.
- Leveraged DDD (Domain-Driven Design) to design the Domain and Bounded Context based on business requirements.
- I personally owned this product and built it single-handedly within 100 days.

𝐈𝐧𝐭𝐞𝐫𝐞𝐬𝐭𝐢𝐧𝐠 𝐟𝐢𝐧𝐝𝐢𝐧𝐠𝐬
- Golang's type alias mechanism is suitable for DDD, as it allows defining rich domain types without the performance or memory footprint of creating complex structs.
- The test strategy is enhanced by DDD because its domain objects are structured as self-contained units, facilitating straightforward unit testing without external dependencies.

𝐅𝐢𝐫𝐬𝐭 𝐒𝐭𝐚𝐠𝐞 𝐅𝐞𝐚𝐭𝐮𝐫𝐞𝐬
- Smart Watchlists for flexible grouping
- An autocomplete search with a ternary search tree from the ground up
- Real-Time Tracking (mocking source)
- Secure Authentication
- Mobile-ready application

𝐇𝐢𝐠𝐡-𝐥𝐞𝐯𝐞𝐥 𝐓𝐞𝐜𝐡𝐧𝐢𝐜𝐚𝐥 𝐃𝐞𝐬𝐢𝐠𝐧
- A monorepo codebase with 15 Golang-based microservices deployable on Kubernetes (K8S)
- High-level design is composed of application-level and infrastructure-level components.
- Explored and implemented critical application-level topics, including: API Design and Versioning, Use Cases and Controllers, Algorithm, Data Query, Concurrency, Error Handling, Testing Strategies, Database Optimization and Selection, and Security.
- Investigated and applied common infrastructure-level principles, such as: Fault Tolerance, High Availability and Scalability, Networking and Protocols, Cloud and DevOps, Monitoring and Observability
- For a detailed explanation of the 'what', please refer to the [LZStock Tech Blog](https://blog.lzstock.app/blog/what-I-built).

𝐋𝐨𝐰-𝐥𝐞𝐯𝐞𝐥 𝐓𝐞𝐜𝐡𝐧𝐢𝐜𝐚𝐥 𝐃𝐞𝐬𝐢𝐠𝐧
- Low-level design topics expand upon high-level concepts, focusing primarily on coding-related aspects, design patterns, and best practices.
- For a detailed explanation of the 'what' and 'how,' please refer to the [LZStock Tech Blog](https://blog.lzstock.app/blog/what-I-built).  

𝐓𝐞𝐜𝐡 𝐒𝐭𝐚𝐜𝐤  
𝘍𝘳𝘰𝘯𝘵 𝘌𝘯𝘥 (react-based)  
➢ Custom Webpack+ Babel stack  
➢  React Hooks/TanStack Router/Jotai/React in Typescript  
➢ Static hosting on Vercel via CircleCI deployment.  
  
𝘚𝘦𝘳𝘷𝘦𝘳 𝘚𝘪𝘥𝘦 (golang-based microservices)  
➢ Golang gRPC Server  
➢ FastHttp as a Gateway  
➢ WebSocket service with gRPC server stream to push session-based stock price  
➢ NATs-JetStream for async-communication  
➢ PostgreSQL, Redis  

𝘋𝘦𝘷-𝘖𝘱𝘴  
➢ CircleCI  
➢ Terraform manage infrastructure configuration  
➢ Helm Chart handle deployments for each service  
➢ Gitlab Container Registry  
➢ K8S on GCP  
➢ GKE + CloudFlare + Vercel  


---

### Data Pipeline: [US Stock Financial Report Dumper](https://github.com/DanielLin9406/worker-financialReportScreenr)
𝐖𝐡𝐚𝐭 𝐢𝐬 𝐭𝐡𝐢𝐬?  
- A streamlined data pipeline that leverages an ETL process to screen companies using raw financial data from Morningstar Excel files, outputting a range of first-level and second-level indicators directly to Google Sheets.

𝐅𝐞𝐚𝐭𝐮𝐫𝐞  
- Modular ETL Pipeline: A clean separation of concerns between Data Ingestion (Local/API), Transformation (Financial Indicator Calculation), and Loading (Google Sheets/Databases).
- Advanced Financial Analysis: Implements various valuation models and indicators, including DCF, Graham Number, DDM, and more.

𝐓𝐞𝐜𝐡 𝐈𝗱𝗲𝗮 
- Robust Design Pattern Implementation: The project leverages a wide array of design patterns (Factory, Observer, Command, Strategy, Builder, Mediator), reflecting advanced proficiency in software architecture and code maintainability.
- Strict Separation of Concerns (SoC): Each architectural layer—from data sources and core calculations to the final delivery—is clearly defined, ensuring modularity and easier debugging.
- Architected for Scalability: By prioritizing ABCs and Strategy patterns, the framework simplifies future enhancements, making it straightforward to add new financial indicators or complex valuation algorithms.
  
𝐓𝐞𝐜𝐡 𝐒𝐭𝐚𝐜𝐤  
𝘚𝘵𝘰𝘳𝘢𝘨𝘦  
➢ Google Sheet  
  
𝘋𝘢𝘵𝘢 𝘗𝘪𝘱𝘦𝘭𝘪𝘯𝘦  
➢ Leverage design patterns such as Factory, Strategy, Mediator, Observer, Chain of Responsibility, and Builder. 

𝐍𝐨𝐭𝐞:  
- A complete version resides in the secFinancialReportScraper folder.  

Skills: Python · Google Sheet API  

---

### Full-stack: [Price Dashboard](https://github.com/DanielLin9406/fullstack-priceDashboard)

𝐖𝐡𝐚𝐭 𝐢𝐬 𝐭𝐡𝐢𝐬?  
- An internal SPA for the purpose of setting and reading prices in terms of each product in the online shop.

𝗪𝗵𝗮𝘁 𝗺𝗮𝗸𝗲 𝘁𝗵𝗶𝘀 𝗽𝗿𝗼𝗷𝗲𝗰𝘁 𝗱𝗶𝗳𝗳𝗲𝗿𝗲𝗻𝘁 𝗳𝗿𝗼𝗺 𝗼𝘁𝗵𝗲𝗿 𝗽𝗲𝗼𝗽𝗹𝗲'𝘀 𝘀𝗶𝗱𝗲 𝗽𝗿𝗼𝗷𝗲𝗰𝘁?   
- A complete full stack project   

𝐅𝐞𝐚𝐭𝐮𝐫𝐞   
- Implemented 3-party API of Google’s spreadsheet API with OAuth2/API keys authorization to my personal website.  

𝐓𝐞𝐜𝐡 𝐈𝗱𝗲𝗮  
- Developed and built up Price Dashboard from a front-end project with SPA feature to a full-stack project with microservice architecture and fully CRUD operations.  
  
𝗧𝗲𝗰𝗵 𝗦𝘁𝗮𝗰𝗸  
𝘍𝘳𝘰𝘯𝘵 𝘌𝘯𝘥  
➢ Custom Webpack+ Babel stack  
➢ React Hooks, React Router, Redux, React SSR, dynamic import  
  
𝘚𝘦𝘳𝘷𝘦𝘳 𝘚𝘪𝘥𝘦  
➢ Node.js Ecosystem: Express, Typescript, Chi+Mocha, Sequelize, Mongoose  
➢ DB/Cache: MongoDB, Redis  

Dev-Ops  
➢ Travis CI  
➢ Container: Docker, Docker-Compose  
➢ Reverse-Proxy: Nginx  
➢ Terraform  

𝘊𝘭𝘰𝘶𝘥  
➢ AWS: ECS  

Skills: JavaScript · Docker · Redis · Travis CI · Mocha (JavaScript Framework) · Webpack · React.js · Mongoose ODM · Nginx · Bash · Node.js

---

### Full-stack: [Email Sender Upgraded](https://github.com/DanielLin9406/fullstack-emailSender-upgraded)
𝐖𝐡𝐚𝐭 𝐢𝐬 𝐭𝐡𝐢𝐬?  
- Upgraded version of a email promotion and monitor system based on Stephergrinder's email sender. Solely to practice the cutting edge tech stack.
  
𝐇𝐨𝐰 𝐢𝐬 𝐭𝐡𝐢𝐬 𝐩𝐫𝐨𝐣𝐞𝐜𝐭 𝐮𝐧𝐢𝐪𝐮𝐞? 
- Learning to build a full-stack proejct

𝐓𝐞𝐜𝐡 𝐈𝗱𝗲𝗮 
- Use Webpack-dev-server to proxy all api services and websocket connection.
- Use express as static file server in production and handle websocket connection.
- A express project in company with graphql+socket.io
- A express project in company with apollo-server+socket.io
- Update api service file structure from technical role to self-contained components.
- Refractor api service from common.js to ES6 import syntax
  
𝐓𝐞𝐜𝐡 𝐒𝐭𝐚𝐜𝐤  
𝘍𝘳𝘰𝘯𝘵 𝘌𝘯𝘥  
➢ Custom Webpack+ Babel stack  
➢ React Hooks, React Router, Redux, dynamic import  
➢ WebSocket by Socket  
➢ Husky+Lint-stage  
  
𝘚𝘦𝘳𝘷𝘦𝘳 𝘚𝘪𝘥𝘦  
➢ Node.js Ecosystem: Express, Chi+Mocha, Mongoose  
➢ WebSocket by Socket.io  
➢ GraphQL by express-graphql or apollo-server  
➢ DB/Cache: MongoDB  
 
𝐒𝐤𝐢𝐥𝐥𝐬: JavaScript · Websocket · Nginx · Docker · Travis CI

---
### Front-End: [Mix Dan Studio](https://github.com/DanielLin9406/frontend-mixDanStudio)
𝐖𝐡𝐚𝐭 𝐢𝐬 𝐭𝐡𝐢𝐬? 
- Refactored version of my very first website with OAuth 2.0 and Google Sheet API integrated.
 
𝐇𝐨𝐰 𝐢𝐬 𝐭𝐡𝐢𝐬 𝐩𝐫𝐨𝐣𝐞𝐜𝐭 𝐮𝐧𝐢𝐪𝐮𝐞? 
- The first task involved transforming a static website into a server-hosted one with third-party API integration.

𝐓𝐞𝐜𝐡 𝐈𝗱𝗲𝗮 
- Multi-entry webpack
- Write a replace image path webpack plugin
- Implement OAuth 2.0 and API keys to authorize user.
- Implement Google Sheet API
 
𝐓𝐞𝐜𝐡 𝐒𝐭𝐚𝐜𝐤
𝘍𝘳𝘰𝘯𝘵 𝘌𝘯𝘥  
➢ Webpack  
➢ Pug template  
➢ WebSocket by Socket  
➢ Husky+Lint-stage  
 
𝘚𝘦𝘳𝘷𝘦𝘳 𝘚𝘪𝘥𝘦  
➢ Express  
➢ Google Sheet API  

Skills: JavaScript · Google Sheet API · Node.js
