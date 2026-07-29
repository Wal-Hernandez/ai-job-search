---
framework_version: 1.3.0
---

# Interview Preparation

<!-- SETUP: These examples are populated by running /setup -->

## Output Location

When running the full job-application workflow, save this interview preparation to:

```
applications/<company>-<role>/interview-notes.md
```

Use the same `<company>-<role>` slug as the CV and cover letter so the application folder is self-contained.

## Candidate: Walter Hernandez

### Behavioral Compass

Quick reference from the candidate's behavioral profile:

- **Primary driver:** building things that are useful and work; satisfaction comes from shipping a feature that makes a user's life genuinely easier.
- **Under pressure:** stays focused, asks directly when a requirement is unclear, and prefers to surface risks early rather than pretend to know everything.
- **Conflict:** responds with facts and evidence, not defensiveness; open to being wrong when a colleague has a better path.
- **Ambition:** become a strong full-stack SSR engineer with backend depth, then move toward AI/data and eventually a leadership role.
- **Ideal team:** competent, transparent, low-politics; values clear requirements and honest feedback.
- **Non-negotiables:** continuous learning, ownership of meaningful work, respect for work-life balance.
- **Likely weakness to address:** impatience when a process feels bureaucratic; tendency to move fast when a teammate needs more context.

Keep this in mind when drafting answers and mock-interview questions.

## Before the interview

1. Re-read the job description and the tailored CV / cover letter you sent.
2. Prepare 2-3 stories that show the role's required skills.
3. Prepare 2-3 thoughtful questions about the role, team, or company.
4. Be ready to explain any career transition or gap in 2-3 sentences.

## Common Interview Categories

### 1. "Tell me about yourself" / Walk me through your CV

**Recommended approach:** Use a concise 1-2 minute narrative that connects the dots to the target role.

> "I'm a full-stack developer with a strong backend orientation. I started out building data and administrative systems at SYNAgro, then moved to Eppical where I worked on AI-powered document analysis, OCR, and integration projects for the insurance and legal sectors. Now at La Nación I'm leading the modernization of a legacy newsletter system, moving it from .NET 2.2 to Node.js and AWS. I enjoy owning backend architecture, designing APIs, and collaborating with product teams. Long-term I'm moving toward AI and data engineering, which is why backend depth and systems thinking matter a lot to me."

### 2. "Why this role / company?"

**Recommended approach:** Pick something concrete from the posting or company that matches your goals and values.

Template answer (customize with company specifics):
> "This role stands out because it combines backend ownership with real product impact. I'm at my best when I can design APIs and architecture that other developers and users actually rely on. I also like that your stack includes [X] and [Y], because I've worked with similar tools and I'm eager to go deeper. Beyond the tech, the team's [transparency / product focus / learning culture] aligns with how I like to work."

### 3. Strengths and weaknesses

**Strength to highlight:** systems thinking + ownership + pragmatic backend delivery.

> "One strength I lean on is translating a vague requirement into a concrete system design. For example, when I joined the newsletter modernization project, the migration path from .NET 2.2 to Node.js was not fully defined. I broke it into phases, mapped the AWS services we needed, and shipped the MVP with a clean data model behind it."

**Weakness to address (with improvement plan):**
> "I can get impatient when a process feels bureaucratic without clear purpose. What I've learned is to pause and ask why the step exists before pushing back. If there's a real compliance or coordination reason, I adapt. If it's wasted motion, I propose a simpler alternative with data. That way I'm not just venting frustration — I'm helping fix it."

### 4. Behavioral / STAR stories

**STAR = Situation, Task, Action, Result.** Keep each story under 90 seconds.

#### Story A: Modernizing a legacy system

**Situation:** At La Nación, the newsletter system ran on a .NET 2.2 codebase with AWS Lambdas and complex dependencies. It was hard to maintain and had no clear migration path.

**Task:** Lead the backend migration to Node.js, define the new architecture, and ensure the system continued serving newsletters without disruption.

**Action:** I broke the work into phases: first I mapped the existing .NET Lambdas and data flow, then proposed a Node.js replacement with AWS services and a clean data model. I built the new backend, designed the APIs, and coordinated with the frontend team so they could integrate incrementally.

**Result:** We delivered a working Node.js backend that replaced the legacy .NET stack, improved maintainability, and gave the team a clear path to extend the product.

#### Story B: Adding AI capabilities to a document-processing pipeline

**Situation:** At Eppical, an insurance client needed to process scanned PDFs and images more efficiently. The existing process was manual and error-prone.

**Task:** Integrate AI-based OCR and document analysis into the product so the client could extract information automatically.

**Action:** I researched and integrated OpenAI APIs for image analysis and PDF text extraction, wired them into the existing Node.js backend, and built the frontend flows in Angular so users could review and validate the extracted data.

**Result:** The client could process documents significantly faster. The feature became part of the core product and influenced the roadmap for the team.

#### Story C: Working with incomplete requirements

**Situation:** A project kicked off with a vague brief: "improve the newsletter system." The scope, success criteria, and deadlines were unclear.

**Task:** Turn the brief into a deliverable backend migration with clear milestones.

**Action:** I asked direct questions — what does "improve" mean, who uses it, what breaks today, and what is the deadline? — then documented the answers, proposed a phased migration, and got alignment before writing code.

**Result:** The team had a clear plan, stakeholders knew what to expect, and we delivered each phase without rework.

### 5. Technical / system design questions

**"How would you design a backend API for a newsletter platform?"**

> "I'd start with the core entities: subscribers, lists, campaigns, templates, and sends. The API would be RESTful with clear resource boundaries. I'd separate read-heavy analytics from write-heavy sends, possibly using a queue for dispatch and tracking events. Auth would be token-based, and I'd version the API from the start. On AWS I'd lean toward API Gateway + Lambda or ECS depending on throughput, DynamoDB or RDS for structured data, and S3 for template assets. I'd also add observability and retries for email provider failures."

**"How do you handle working with a legacy codebase?"**

> "First I understand what it does and why it exists — I read the code, run it, and talk to people who know it. Then I identify the riskiest or most painful parts. I prefer incremental migration over big-bang rewrites: define boundaries, write tests around the existing behavior, replace one module at a time, and validate each step in production. Communication matters too — legacy rewrites often fail because the business doesn't understand why the team is slow for a while."

**"Tell me about a time you had to debug a hard production issue."**

> "We had a case where newsletter sends were intermittently failing. The logs were noisy because the legacy .NET Lambdas didn't have consistent tracing. I added structured logging and request correlation IDs, then narrowed it down to a timeout in an external email provider call. I added retries with exponential backoff and a dead-letter queue for failures. After that, we could see the issue clearly and recover automatically."

### 6. "What do you know about our company?"

**Always do research before the interview.** Read the company's homepage, recent press or blog posts, and the team page if available. Prepare 2-3 specific facts that connect to the role.

Template:
> "I know you [recent product launch / market focus / tech stack]. What I find interesting is [specific detail]. It seems like the engineering team is focused on [scalability / customer experience / data quality], which is exactly the kind of work I want to do more of."

### 7. Salary expectations

**Do not give a hard number in the first call.** Instead, give a range based on market research and your needs.

Template:
> "Based on my research of salaries for backend/full-stack SSR roles in [region], and considering my experience with Node.js, .NET, AWS, and AI integration, I'm looking for a range around [X] to [Y]. I'm flexible on the exact mix of base, benefits, and growth opportunities, and I'd love to understand your compensation structure first."

User preference: salary and references are not included in the profile by default; only include if explicitly requested.

### 8. Questions to ask the interviewer

Prepare 2-3 questions from this list, tailored to the company:

- What does success look like in this role in the first 3-6 months?
- How is the engineering team structured? Who would I work most closely with?
- What is the current biggest technical challenge the team is facing?
- How do you handle technical debt and legacy code?
- What does the onboarding process look like?
- How do you measure the impact of a feature or backend improvement?
- What opportunities are there for learning and growth, especially in backend or AI/data?

## Post-interview follow-up

Send a short thank-you email within 24 hours. Reference one specific topic from the conversation.

Template:
> "Hi [Name], thank you for taking the time to speak with me today. I enjoyed learning about [specific topic], and I'm even more interested in the role. Please let me know if there's anything else you need from me. Best, Walter"

## Last-minute check

Before the interview, confirm:

- [ ] Job description and CV / cover letter reviewed
- [ ] 2-3 STAR stories prepared
- [ ] 2-3 questions ready for the interviewer
- [ ] Company facts researched
- [ ] Technical talking points prepared for the stack listed in the job ad
- [ ] Salary range researched (if applicable)
- [ ] Calendar / link / interview time confirmed
