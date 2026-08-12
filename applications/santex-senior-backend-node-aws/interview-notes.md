# Interview Notes: Santex — Senior Backend Developer (Node & AWS)

## STAR Stories

### AWS migration and serverless deployment (La Nación)
- **Situation:** La Nación relied on a legacy .NET 2.2 newsletter system running on aging infrastructure that was hard to maintain and scale.
- **Task:** Lead the migration from the legacy system to a modern Node.js + AWS serverless architecture.
- **Action:** Designed the REST API contract and data model. Implemented the Node.js backend and deployed serverless workflows on AWS Lambda and API Gateway. Coordinated with Architecture, Database and Frontend teams on integration points.
- **Result:** Replaced the legacy pipeline with a maintainable, cloud-native backend. Later promoted to core developer on the Paywall monorepo.

### AI-integrated backend workflow (Eppical)
- **Situation:** A client required document analysis automation within an existing workflow that had no AI capabilities.
- **Task:** Build a backend integration that routes documents to OpenAI APIs and returns structured analysis results to the frontend.
- **Action:** Developed Node.js/.NET services to handle routing and result processing. Built Angular UI components. Collaborated with the team to evaluate technical trade-offs on API design and data flow.
- **Result:** A working AI-assisted document-analysis pipeline integrated into the product's Angular frontend.

### Production debugging and cross-system fixes (SYNAgro)
- **Situation:** Customer-facing agribusiness applications had recurring production bugs across React, Ionic and .NET layers.
- **Task:** Diagnose root causes and fix bugs across the full stack while maintaining feature velocity.
- **Action:** Built responsive web and mobile interfaces with React, TypeScript and Ionic. Wrote C#/.NET backend services and SQL database changes. Fixed production bugs by tracing issues through the full stack.
- **Result:** Improved application stability and delivered customer-facing features such as email layouts. This is where I learned to debug production incidents systematically — relevant to the on-call rotation in this role.

## Likely Questions

### Technical
1. Describe the AWS services you have used in production. What was your role in provisioning them?
2. How do you approach designing a REST API for a new integration product?
3. Walk me through an event-driven architecture you have worked with or designed.
4. What is your experience with SQL Server vs. PostgreSQL? When would you choose one over the other?
5. How do you ensure code quality across multiple repositories in a CI/CD pipeline?
6. Have you used Terraform or any infrastructure-as-code tool? Be honest — what would your ramp-up look like?
7. Describe a time you debugged a production incident. What was your process?
8. How do you test serverless applications?

### Behavioral
1. Tell us about a time you worked across multiple codebases or systems simultaneously.
2. How do you handle shifting sprint priorities?
3. Describe your experience with on-call rotations or after-hours incident response.
4. How do you collaborate with QA and SDETs to ensure thorough testing?
5. Give an example of a time you made an architectural decision within a defined scope.

### Logistics
1. Are you based in Argentina?
2. What is your English level?
3. What are your salary expectations?
4. Are you available for on-call rotation and off-hours deployments?

## Talking Points
- Strong Node.js + AWS serverless production experience at La Nación.
- Both SQL Server and PostgreSQL experience — comfortable with multi-database environments.
- Azure DevOps CI/CD pipelines as current toolset.
- AI tooling experience: OpenAI API integration at Eppical + Copilot/Cursor for daily development.
- SOLID principles and design patterns applied in production backend code.
- Terraform: actively learning, strong AWS fundamentals make ramp-up fast.
- Argentina-based, remote-ready, C1 English.

## Gaps to Address Honestly
- **Terraform:** Not in production toolset. Actively learning. Position it as: "I understand what Terraform solves because I have provisioned AWS services manually. I am ready to adopt it quickly and will be productive within weeks, not months."
- **Event-driven architecture at scale:** Your AWS serverless work touches event-driven patterns (Lambda invocations) but you have not designed large-scale event-driven systems. Be honest: "I have worked with event-driven patterns through AWS Lambda and understand the principles. I am ready to deepen this skill."
- **Microservices:** Your experience is more modular monolith/API-driven than fully distributed microservices. Say: "I have designed APIs with separation of concerns, which is the foundation of microservices architecture. I understand the trade-offs around data consistency, service boundaries and inter-service communication."

## Questions to Ask
1. How is work distributed across the three codebases (Data Integration, payments, APIs)? What percentage is Node.js/AWS vs. SQL Server?
2. What does the on-call rotation look like — frequency, typical incident volume?
3. What does the engineering team size and composition look like?
4. How does Santex support professional development — are there internal learning paths for infrastructure as code or AWS certification?
5. What are the biggest technical challenges the integration team is facing right now?
