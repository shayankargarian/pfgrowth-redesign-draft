# IA / UX critique and proposed information architecture

## What’s wrong with the current experience

### Information architecture
1. **Partner blocks dominate every page.** SVB / IFC / IDB content repeats under homepage, what-we-do, connect, team, portfolio, disclosures. It dilutes page-specific goals and makes length feel like filler.
2. **Overlapping “product” pages.** `/what-we-do/`, `/discover-growth-debt/`, and homepage “What We Do” all explain growth debt with different depth and tone. Users cannot tell which is canonical.
3. **Portfolio is a wall.** A near-alphabetical dump of hundreds of companies overwhelms mobile users. Featured stories exist but compete with the directory instead of leading it.
4. **Nav labels are institutional, not task-led.** “Who We Are / What We Do / Global Portfolio / Team / Connect” mirrors org chart language more than founder questions (“Am I a fit?”, “What do I get?”, “Talk to someone”).
5. **Secondary programmes float.** Tech CFO Connect, careers, news, timeline, ESG webinar are hard to place in a clear journey for primary borrowers.
6. **Legacy / duplicate URLs** in sitemap (`global-portfolio-2`, `-4`) signal unfinished IA cleanup.

### UX and conversion
1. **Primary CTA is soft.** “Sign up for updates” competes with (and often outweighs) “speak to a partner about financing.” Newsletter is not the money path.
2. **Fit criteria buried.** Revenue, ticket size, and structures sit mid-page on What We Do. Founders need a scannable “Is this for us?” early.
3. **Mobile hierarchy struggles.** Elementor-heavy layout, repeated footers, and long comparison tables do not prioritise thumb-reach CTAs or short sections.
4. **Credibility without clarity.** 35 years and global offices are strong, but the homepage does not lead with the financing outcome in plain language.
5. **Contact friction.** Offices listed well; clear phone/email hierarchy and “who to contact by region or need” is weak on the public connect page.
6. **Accessibility risk.** Heavy motion/counters, dense partner copy, and repeated forms increase cognitive load; focus order and contrast need deliberate redesign.

## Proposed IA (prototype scope)

Phone-first sitemap for the redesign prototype:

```
Home (/)
├── Growth debt (/growth-debt.html)     ← product + fit criteria + structures
├── Proof (/portfolio.html)             ← curated stories + sectors + regions
├── About (/about.html)                 ← story, belief, leadership, partners (once)
└── Connect (/contact.html)             ← lead form, offices, regional routing
```

Footer only: Important disclosures (summary + link note), privacy note. News, careers, Tech CFO Connect deferred as phase-2 links in footer “More” (not competing with primary nav).

### Page goals

| Page | User question answered | Primary CTA | Success metric (concept) |
| --- | --- | --- | --- |
| Home | What is PFG and why talk now? | Start a conversation | Scroll to fit band + CTA tap |
| Growth debt | Is this for my company? What can I raise? | Check fit / talk to us | Time on criteria + CTA |
| Proof | Who have you backed like me? | Talk about our stage | Story engagement |
| About | Can I trust this team? | Meet the Sydney / global team | Leadership skim |
| Connect | How do I reach the right person? | Submit enquiry | Form completion |

### Journey we optimise for
1. Land on Home → understand **growth debt in one screen**.
2. Confirm **fit** (revenue, ticket, sector) on Growth debt.
3. Build confidence via **2-3 relevant stories** (not 200 logos).
4. **Connect** with region + need fields (borrower vs LP vs media).

### Content principles for the rewrite
- One explanation of growth debt; cut duplicate essays.
- Partners appear once (About), not as a sitewide appendix.
- Portfolio = curated proof first; full directory is phase 2.
- Australian English; short sentences; no em dashes.
- Every page ends with the same primary CTA pattern.
