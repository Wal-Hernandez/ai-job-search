# Interview Notes: Avenga — Middle/Senior NodeJS Engineer

## STAR Stories

### Event-driven migration with CDK (La Nación)
- **Situation:** La Nación's legacy .NET 2.2 newsletter system could not scale with the company's growth and was hard to maintain.
- **Task:** Contribute to the migration to a Node.js + AWS event-driven architecture, building backend microservices and provisioning cloud infrastructure.
- **Action:** Built event-driven backend services integrated via EventBridge and SQS. Provisioned AWS infrastructure using CDK. Configured Dead Letter Queues for fault tolerance and set up CloudWatch monitoring. Explored Step Functions as part of the migration's planned evolution. Deployed through Azure DevOps CI/CD.
- **Result:** Replaced the legacy system with a scalable, observable event-driven architecture. Later evolved into a core developer on the Paywall monorepo.

### Production debugging across event-driven services (La Nación)
- **Situation:** Production issues arose in the event-driven newsletter system requiring tracing across EventBridge, Lambda and downstream services.
- **Task:** Identify root causes of failures in the event pipeline.
- **Action:** Traced events through EventBridge rules, Lambda execution logs and CloudWatch. Used DLQ messages to identify failed event processing and resolve the underlying issues.
- **Result:** Resolved production bugs by systematically tracing events across services. This experience applies directly to debugging event-driven architectures.

### AI-integrated backend workflow (Eppical)
- **Situation:** A client required document analysis automation within an existing workflow.
- **Task:** Build a backend integration routing documents to OpenAI APIs and returning structured analysis results.
- **Action:** Developed Node.js/.NET services for routing and result processing. Built Angular frontend components. Collaborated with the team on API design trade-offs.
- **Result:** Working AI-assisted document-analysis pipeline integrated into the product.

## Likely Questions

### Technical
1. Describe an event-driven architecture you have worked on. How did services communicate?
2. What is your experience with Infrastructure as Code? Which tools have you used?
3. How do you handle error handling and fault tolerance in event-driven systems?
4. Walk me through how you debug a production issue in an event-driven architecture.
5. What is your experience with NoSQL databases? Which ones?
6. Describe a REST API you designed. What patterns did you use?
7. What is your experience with CI/CD pipelines?
8. Have you used Step Functions or similar orchestration tools?
9. How do you approach scalability and high availability in your designs?
10. What is your experience with TypeScript?

### Behavioral
1. How do you work within a Scrum team with DevOps and Product Owners?
2. Describe a time you collaborated across teams to solve a complex problem.
3. How do you handle shifting priorities in an agile environment?
4. Tell us about a time you had to learn a new technology quickly.

### Domain
1. Do you have experience in banking or financial services? (Answer: No, but willing to learn. Emphasize that event-driven, scalable, and reliable architectures are domain-agnostic skills.)

## Talking Points
- Node.js backend with event-driven architecture at La Nación — EventBridge, SQS, Lambda, CloudWatch.
- AWS CDK for Infrastructure as Code — IaC experience in practice.
- MongoDB for NoSQL — meets the requirement.
- TypeScript in daily use — covers the nice-to-have.
- REST API design across multiple roles.
- CI/CD with Azure DevOps pipelines.
- Step Functions: explored and participated in implementation but not owned in production. Honest about scope.
- Banking domain: new to me, but my architecture skills transfer. Eager to learn.

## Gaps to Address Honestly
- **Step Functions:** Explored as part of the migration's planned evolution. Participated in the implementation effort but did not own a production workflow. Be clear: "I studied Step Functions, participated in the implementation, and understand the orchestration model. I am ready to build production workflows with it."
- **SNS and DynamoDB:** Not in my toolkit. SQS and EventBridge cover the messaging concepts. MongoDB covers NoSQL concepts.
- **Banking domain:** No prior experience. Frame as: "I am experienced in building scalable, reliable architectures — the qualities that matter in banking. I learn domains quickly."

## Questions to Ask
1. What does the banking client's architecture look like — how are event-driven patterns used?
2. What is the team size and composition?
3. How does Avenga support professional development and certification (e.g., AWS)?
4. What are the biggest technical challenges the team is currently facing?
5. How is work distributed between feature development, maintenance, and production support?
