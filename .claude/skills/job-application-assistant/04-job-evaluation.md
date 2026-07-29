---
framework_version: 1.1.0
---

# Job Evaluation Framework

<!-- SETUP: Skill match areas and career goals are personalized by running /setup -->

## Eligibility Gate — run before scoring

Walter is based in Argentina and is open to remote, hybrid, and international opportunities. If a posting requires citizenship or permanent residency in a specific country, read the posting's eligibility section verbatim and classify. Silence on citizenship/residency is not permission; flag as unverified and proceed with caution.

| Posting wording | Verdict |
|-----------------|---------|
| Names a citizenship or permanent-residency requirement | FAIL — hard stop |
| Requires a security clearance | FAIL in most countries |
| Explicitly accepts Argentina / LATAM / international / remote / visa sponsorship | PASS |
| Silent on citizenship or residency | PROCEED, but mark unverified |

## Scoring Dimensions

Evaluate each job posting against these five dimensions:

### 1. Technical Skills Match (0-100)
How well do the required/preferred skills align with Walter's capabilities?

| Score | Meaning |
|-------|---------|
| 80-100 | Core requirements are primary skills (Node.js, .NET, backend architecture, API design) |
| 60-79 | Most requirements match, 1-2 gaps that are learnable |
| 40-59 | Partial match, significant upskilling needed |
| 0-39 | Fundamental mismatch |

**Strong match areas:** Node.js, TypeScript, C#, .NET, backend development, REST API design, SQL Server, MongoDB, AWS, Azure, React, Angular.
**Moderate match areas:** Docker, Kubernetes, AI/ML integration, Python, data pipelines, distributed systems.
**Weak match areas:** Advanced machine learning, data science, deep learning, specialized frontend-only roles.

### 2. Experience Match (0-100)
Does work history align with what they're looking for?

| Score | Meaning |
|-------|---------|
| 80-100 | Direct experience in the same domain and role type |
| 60-79 | Related experience, transferable skills clear |
| 40-59 | Adjacent experience, would need to make the case |
| 0-39 | Unrelated experience |

**Strong:** Full stack development, backend-focused roles, media/newsletter/paywall systems, legacy modernization, AI integration, API design, cloud infrastructure.
**Moderate:** SaaS platforms, fintech, cybersecurity, data engineering roles.
**Entry-level:** Pure data science, ML research, frontend-only roles.

### 3. Behavioral/Culture Fit (0-100)
Does the role and company culture match Walter's behavioral profile?

| Score | Meaning |
|-------|---------|
| 80-100 | Culture strongly matches behavioral preferences |
| 60-79 | Mixed signals but mostly compatible |
| 40-59 | Some friction areas |
| 0-39 | Significant culture mismatch |

**Red flags to research:** Heavy people-management requirements, siloed execution without collaboration, no technical discussion or code review culture, rigid tech stack without learning opportunities.

### 4. Location & Logistics (Pass/Fail + Notes)
- Remote from Argentina: PASS
- Hybrid with LATAM office: PASS
- Relocation required: FLAG (discuss with Walter)
- Citizenship/visa barrier: FAIL

### 5. Career Alignment & Motivation (0-100)
Does this role advance career goals and contain tasks that energize?

| Score | Meaning |
|-------|---------|
| 80-100 | Strongly aligned with backend architecture and AI/data growth path |
| 60-79 | Good role but only partially aligned with long-term goals |
| 40-59 | Decent job but doesn't build toward AI/data direction |
| 0-39 | Dead end or backwards step |

**Career goals:**
- Short term: Full Stack Developer SSR or Backend Developer SSR with backend/architecture focus.
- Medium term: Combine backend expertise with AI, ML, data engineering, and automation.
- Long term: AI engineer / data engineer / backend architect solving complex problems.

**Motivation filter:**
- Tasks that energize: backend architecture, API design, legacy modernization, AI integration, technical discussions, code reviews, cross-functional collaboration, learning new technologies.
- Tasks that drain: pure frontend-only execution, extensive people management, isolated work without technical feedback, maintenance without growth.
- Non-task factors: learning culture, technical mentorship, autonomy, team quality, modern tooling.

**Life situation alignment:**
- **Security:** Currently employed at La Nación; can evaluate offers carefully.
- **Flexibility:** Remote preferred; hybrid acceptable; open to international opportunities.
- **Professional development:** Prioritizes roles with technical growth, AI/data exposure, and architecture opportunities.

### 6. Salary Benchmark (Optional)

If the salary lookup tool is configured (`salary_data.json` exists), look up the company:
```
python salary_lookup.py "<Company Name>" --json
```

If a city is known from the posting, add `--city "<City>"` to narrow results.

Walter has chosen not to set a fixed salary expectation in the profile. Present benchmarks as context, not as a target.

## Output Format

Present the evaluation as:

```
## Job Fit Evaluation: [Role] at [Company]

| Dimension | Score | Notes |
|-----------|-------|-------|
| Technical Skills | XX/100 | [brief note] |
| Experience Match | XX/100 | [brief note] |
| Behavioral Fit | XX/100 | [brief note] |
| Location | PASS/FAIL | [brief note] |
| Career Alignment | XX/100 | [brief note] |

**Overall Score: XX/100** (weighted average of scored dimensions)

### Verdict: [Strong Fit / Good Fit / Moderate Fit / Weak Fit / Poor Fit]

### Key Strengths for This Role
- [bullet points]

### Gaps to Address
- [bullet points]

### Recommendation
[1-2 sentences: apply/skip/apply with caveats]

### Company Research Checklist
- [ ] Checked company website (mission, values, recent news)
- [ ] Checked review sites (Glassdoor, LinkedIn, etc.)
- [ ] Checked LinkedIn for team size, recent hires, connections
- [ ] Checked media for restructuring, growth, or workplace issues
- [ ] Identified network contacts who may know the team/manager
```

## Weighting
- Technical Skills: 30%
- Experience Match: 25%
- Behavioral Fit: 15%
- Career Alignment: 30%

(Location is pass/fail, not weighted)

## Thresholds
- **Strong Fit** (75+): Definitely apply, tailor everything
- **Good Fit** (60-74): Apply, address gaps in cover letter
- **Moderate Fit** (45-59): Consider carefully, discuss with Walter
- **Weak Fit** (30-44): Probably skip unless strategic reasons
- **Poor Fit** (<30): Skip

## Pre-Application: Call the Employer (Best Practice)

Before writing the application, consider whether Walter should call the contact person listed in the posting. Only call if there are substantive questions - never call just to "be remembered."

### When to Suggest Calling
- The posting has unclear or ambiguous requirements
- It's unclear which competencies are essential vs. nice-to-have
- The role description is vague about day-to-day tasks
- There's a named contact person who invites questions

### Good Questions to Ask
- "What are the primary challenges in this role?"
- "How is time typically divided across the listed responsibilities?"
- "Which competencies are most critical for success in this position?"
- "What does success look like in the first 6-12 months?"

### Rules for the Call
- Prepare a 30-second elevator pitch about background
- The call's purpose is gathering information, not delivering a pitch
- Take notes and use what you learn to tailor the application
- Reference the conversation naturally in the cover letter
