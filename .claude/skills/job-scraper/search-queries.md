# Search Queries for Job Scraper

<!-- SETUP: Customized for Walter Hernandez - Full Stack / Backend SSR, remote-first -->

## Geographic Priority (run searches in this order)

1. **Argentina** — ideal if on-site/hybrid; Walter is based in Argentina.
2. **LATAM Remote** — second best; strong timezone overlap and common remote market.
3. **International Remote** — third; worldwide distributed teams.

The scraper should run queries in the order below and present results grouped by geography, keeping the same order. Within each geography, run role priorities 1 → 2 → 3.

## Installed portal CLIs (primary for `/scrape`)

`/scrape` discovers every portal skill under `.agents/skills/*/SKILL.md` and runs its CLI first. Shipped country-agnostic CLIs include `linkedin-search` and `freehire-search`; Danish demos and any skill you add with `/add-portal` are included the same way. You do **not** need a matching `site:` line below for those CLIs to run.

The `site:` query templates in this file are the **WebSearch fallback** — for portals without a CLI, company career pages, or when a CLI fails.

## Search Sites

Primary:
- **linkedin.com/jobs** - LinkedIn job listings (filter: Remote / Argentina / Worldwide); also covered by `linkedin-search` CLI
- **freehire.me** - Aggregator covering ~50 ATS platforms; also covered by `freehire-search` CLI
- **getonbrd.com** - Latin American tech job board
- **ticjob.es** / **tecnoempleo.com** - Spanish-speaking tech boards (remote-friendly)

Secondary (company career pages via Google):
- Direct Google searches with `site:` filters for known target companies

## Query Categories

Queries are grouped by geography first, then role priority. Each query should be combined with the location/work-mode terms that the site supports.

### Geography A: Argentina (highest priority)

#### Priority 1: Full Stack / Backend SSR in Argentina

```
site:linkedin.com/jobs "Full Stack Developer" Argentina
site:linkedin.com/jobs "Full Stack Engineer" Argentina
site:linkedin.com/jobs "Backend Developer" Argentina
site:linkedin.com/jobs "Backend Engineer" Argentina Buenos Aires
site:freehire.me "Full Stack Developer" --country AR
site:freehire.me "Backend Developer" --country AR
site:getonbrd.com "Full Stack Developer" Argentina
site:getonbrd.com "Backend Developer" Argentina
```

#### Priority 2: JavaScript / TypeScript / Node.js / .NET in Argentina

```
site:linkedin.com/jobs "Node.js Developer" Argentina
site:linkedin.com/jobs "TypeScript Developer" Argentina
site:linkedin.com/jobs ".NET Developer" Argentina
site:linkedin.com/jobs "JavaScript Developer" Argentina
site:freehire.me "Node.js" --country AR
site:freehire.me "TypeScript" --country AR
site:freehire.me ".NET" --country AR
site:getonbrd.com "Node.js" Argentina
site:getonbrd.com "React" Argentina
```

#### Priority 3: AI / Data Engineering Adjacent in Argentina

```
site:linkedin.com/jobs "AI Engineer" Argentina
site:linkedin.com/jobs "Machine Learning Engineer" Argentina
site:linkedin.com/jobs "Data Engineer" Argentina
site:freehire.me "AI Engineer" --country AR
site:freehire.me "Data Engineer" --country AR
site:getonbrd.com "Data Engineer" Argentina
```

### Geography B: LATAM Remote (second priority)

#### Priority 1: Full Stack / Backend SSR remote in LATAM

```
site:linkedin.com/jobs "Full Stack Developer" remote LATAM
site:linkedin.com/jobs "Full Stack Engineer" remote Latin America
site:linkedin.com/jobs "Backend Developer" remote LATAM
site:linkedin.com/jobs "Backend Engineer" remote Latin America
site:freehire.me "Full Stack Developer" --remote remote --region latam
site:freehire.me "Backend Developer" --remote remote --region latam
site:getonbrd.com "Full Stack Developer" remoto LATAM
site:getonbrd.com "Backend Developer" remoto LATAM
```

#### Priority 2: JavaScript / TypeScript / Node.js / .NET remote in LATAM

```
site:linkedin.com/jobs "Node.js Developer" remote LATAM
site:linkedin.com/jobs "TypeScript Developer" remote Latin America
site:linkedin.com/jobs ".NET Developer" remote LATAM
site:freehire.me "Node.js" --remote remote --region latam
site:freehire.me "TypeScript" --remote remote --region latam
site:freehire.me ".NET" --remote remote --region latam
site:getonbrd.com "Node.js" remoto LATAM
site:getonbrd.com "React" remoto LATAM
```

#### Priority 3: AI / Data Engineering Adjacent remote in LATAM

```
site:linkedin.com/jobs "AI Engineer" remote LATAM
site:linkedin.com/jobs "Machine Learning Engineer" remote Latin America
site:linkedin.com/jobs "Data Engineer" remote LATAM
site:freehire.me "AI Engineer" --remote remote --region latam
site:freehire.me "Data Engineer" --remote remote --region latam
site:getonbrd.com "Data Engineer" remoto LATAM
```

### Geography C: International Remote (third priority)

#### Priority 1: Full Stack / Backend SSR remote worldwide

```
site:linkedin.com/jobs "Full Stack Developer" remote
site:linkedin.com/jobs "Full Stack Engineer" remote worldwide
site:linkedin.com/jobs "Backend Developer" remote
site:linkedin.com/jobs "Backend Engineer" remote
site:freehire.me "Full Stack Developer" --remote remote
site:freehire.me "Backend Developer" --remote remote
site:getonbrd.com "Full Stack Developer" remoto internacional
site:getonbrd.com "Backend Developer" remoto internacional
```

#### Priority 2: JavaScript / TypeScript / Node.js / .NET remote worldwide

```
site:linkedin.com/jobs "Node.js Developer" remote
site:linkedin.com/jobs "TypeScript Developer" remote
site:linkedin.com/jobs ".NET Developer" remote
site:linkedin.com/jobs "JavaScript Developer" remote
site:freehire.me "Node.js" --remote remote
site:freehire.me "TypeScript" --remote remote
site:freehire.me ".NET" --remote remote
site:getonbrd.com "Node.js" remoto
site:getonbrd.com "React" remoto
```

#### Priority 3: AI / Data Engineering Adjacent remote worldwide

```
site:linkedin.com/jobs "AI Engineer" remote
site:linkedin.com/jobs "Machine Learning Engineer" remote
site:linkedin.com/jobs "Data Engineer" remote
site:freehire.me "AI Engineer" --remote remote
site:freehire.me "Data Engineer" --remote remote
site:getonbrd.com "Data Engineer" remoto
```

### Priority 4: Cloud / DevOps / Technical Consulting

Wider net for technical roles where backend experience transfers.

```
site:linkedin.com/jobs "AWS Developer" remote
site:linkedin.com/jobs "Azure Developer" remote
site:linkedin.com/jobs "Software Engineer" remote Argentina
site:linkedin.com/jobs "Technical Consultant" remote
site:freehire.me "Software Engineer" --remote remote
site:freehire.me "Cloud Engineer" --remote remote
site:getonbrd.com "Software Engineer" remoto
```

## Location Filter

Preferred work arrangements and locations:
- **Argentina (Buenos Aires / CABA / Gran Buenos Aires)** — ideal for on-site/hybrid
- **Remote (Argentina)** — ideal
- **Remote (LATAM)** — second best
- **Remote (worldwide)** — third best
- **Hybrid in Buenos Aires / Gran Buenos Aires** — acceptable
- **On-site in Buenos Aires / CABA** — acceptable if the role is strong
- **Other provinces in Argentina** — case by case
- **On-site outside Argentina** — too far unless relocation is explicitly desired

## Date Filter

Only include jobs posted within the last 14 days, or with an application deadline that has not yet passed. If a posting date cannot be determined, include it but flag as "date unknown".

## Adapting Queries

If the user specifies a focus area, select queries from the matching category across all three geographies, keeping the Argentina → LATAM → International order. For example:
- "/scrape backend" → Priority 1 backend queries in Argentina, then LATAM, then International.
- "/scrape AI" → Priority 3 AI/data queries in Argentina, then LATAM, then International.
- "/scrape Argentina" → Run all Argentina queries only.

When presenting results, sort first by geography (A, B, C), then by fit (high, medium, low), then by date (newest first).
