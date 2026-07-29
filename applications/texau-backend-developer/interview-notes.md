# Interview Notes: Backend Developer at TexAu

## Role and Company Context

- **Role:** Backend Developer
- **Company:** TexAu — growth automation platform (lead generation, data extraction, outbound workflows)
- **Work mode:** Remote, fully distributed
- **Primary language:** English
- **Key stack:** Node.js, Docker, Kubernetes, APIs, serverless functions
- **Key gaps to address:** Docker/Kubernetes production, open-source contributions, web scraping

## Behavioral Compass Quick Reference

- Driven by building useful, working systems.
- Performs well with autonomy balanced by team feedback.
- Prefers technical ownership over people management.
- Learns through code reviews and technical discussion.
- Potential friction: impatience with bureaucracy; English B1 for primary-language team.

## Prepared Answers

### 1. Tell me about yourself

> "I am a backend-focused full-stack developer with 4+ years of production experience. I started building ERP and administrative systems at SYNAgro, then moved to Eppical where I built AI-powered document analysis pipelines. Now at La Nación I am leading the migration of a legacy .NET newsletter system to Node.js and AWS serverless. I enjoy owning backend features end to end, and I am looking for a remote role where I can deepen my work in automation, APIs, and scalable systems."

### 2. Why TexAu?

> "TexAu is an automation and data-pipeline platform, which is exactly the kind of backend problem I want to work on. I also like that you are fully distributed and API-first, because that matches how I work best: with clear technical ownership and strong written communication."

### 3. Why this role?

> "This role sits at the intersection of what I already do well — Node.js backends, AWS, and API design — and what I want to grow into: automation pipelines, serverless architectures, and distributed systems. The team seems to value self-starters, which fits how I like to work."

### 4. Describe your experience with Node.js and AWS

Use the La Nación STAR story:

- **Situation:** Legacy newsletter system running on .NET 2.2 with AWS Lambdas and complex dependencies.
- **Task:** Lead backend migration to Node.js, define new architecture, keep newsletter operations running.
- **Action:** Mapped existing .NET Lambdas and data flow, proposed a Node.js replacement with AWS services and a clean data model, built the new backend and APIs, coordinated incremental frontend integration.
- **Result:** Delivered a working Node.js backend that replaced the legacy .NET stack, improved maintainability, and gave the team a clear path to extend the product.

### 5. What is your experience with Docker and Kubernetes?

> "I have used Docker in learning environments and am actively expanding that knowledge. My production deployment experience is currently centered on AWS serverless (Lambda, S3, API Gateway), so I understand the deployment lifecycle and observability concerns. I am confident I can ramp up quickly on containerized workflows, and I am already studying Kubernetes as part of my security/infrastructure coursework."

### 6. How do you handle working in a fully remote team?

> "I have worked remotely at Eppical and La Nación. I rely on clear written updates, asking questions early when requirements are incomplete, and keeping documentation current. I also make sure to surface blockers rather than silently spin. The 4–5 hour overlap window TexAu mentions is workable from Argentina."

### 7. Tell me about a time you had to debug a hard production issue

> "We had intermittent newsletter send failures in the legacy system. The logs were noisy, so I added structured logging and request correlation IDs, narrowed the issue to a timeout in an external email provider call, and added retries with exponential backoff plus a dead-letter queue. After that, failures became visible and recoverable automatically."

### 8. Tell me about a time you worked with unclear requirements

Use the unclear-requirements STAR story from La Nación:

- **Situation:** Brief said "improve the newsletter system" with unclear scope and success criteria.
- **Task:** Turn the brief into a deliverable backend migration with milestones.
- **Action:** Asked direct questions about users, pain points, deadlines, documented answers, proposed a phased migration, got alignment before coding.
- **Result:** Clear plan, stakeholder expectations set, delivered each phase without rework.

## Questions to Ask the Interviewer

1. What does the backend team structure look like, and who would I work with most closely?
2. What are the current main technical challenges in the platform?
3. How do you handle the 4–5 hour overlap requirement for this role?
4. What does on-call and production incident handling look like?
5. Are there opportunities to work with Kubernetes and automation pipelines?
6. What would success look like in the first 3–6 months?
7. How do you prioritize work between the no-code spreadsheet product, the REST API, and the MCP server?

## Follow-up Plan

- Send a short thank-you email within 24 hours referencing one specific topic from the conversation.
- Keep this file updated with any new information learned during the interview.
