# User Research & Problem Validation Framework

## Framework Overview

User research is the foundation for building AI products that solve real problems. Unlike traditional software, AI products require deep understanding of user workflows, pain points, and the specific data patterns that will drive model performance. This framework helps you systematically validate that you're building for a genuine problem with sufficient demand, and that your understanding of user context will inform critical decisions downstream—from data collection strategy to model requirements to your product roadmap.

## When to Use

Conduct this research at the start of any new product initiative or when entering a new market segment. Plan for 2-4 weeks of primary research (interviews, observation, surveys) combined with secondary research. This work directly informs three downstream deliverables: your data strategy (what data you need to collect and train), your model requirements spec (what capabilities the model must have), and your PRD (how users will actually interact with the product). Skipping or rushing this phase typically leads to building features users don't need or discovering mid-development that your data assumptions were wrong.

---

## Key Sections: Blank Template

Use this template as a starting point for your own user research. Replace each section with your findings.

### User Demographics & Segments

Define who you're building for and why they're different from each other.

**Primary Segment(s):**
- Job title and company type
- Company size range
- Industry or use case
- Geographic scope
- Market size estimate (TAM, SAM, or user count)

**Secondary Segment(s):**
- Adjacent users who might benefit
- Why they're secondary vs. primary

---

### Problem Definition

Describe the specific problem your product will address.

**The Problem:**
- How users currently spend their time on this task
- What tools or workarounds they use today
- Why those solutions are inadequate

**Quantifying the Problem:**
- Time spent per week/month on this task
- Financial cost or opportunity cost
- Frequency and impact of failures or bottlenecks

---

### Validation Evidence

Show that this problem is real and worth solving.

- Number of interviews conducted and target segment
- Key quotes or findings from research
- Percentage of interviewees who confirmed this problem
- Willingness to pay or budget allocation data
- Competitive alternatives and why they fall short

---

### User Context & Constraints

Understand how the problem fits into users' actual work environment.

- Where and when the task happens
- Time pressure and deadlines
- Other tools and systems they use
- Brand, compliance, or quality constraints
- Team structure and decision-making

---

### Success Criteria

Define what "solved" looks like from the user's perspective.

- Specific metrics (speed, quality, accuracy, consistency)
- Qualitative improvements (ease of use, confidence)
- Adoption barriers and how you'll overcome them
- Integration requirements with existing systems

---

## Realistic Example: AI Writing Assistant

### Context

**Company:** Marcom AI

**Product:** An AI writing assistant designed to help marketing teams create on-brand content faster.

---

### User Demographics & Segments

**Primary Segment: In-House Content Marketing Teams**

We're targeting mid-market B2B SaaS and technology companies with content marketing operations. Our primary users are content marketing managers, strategists, and individual content creators within these organizations.

- **Job titles:** Content Marketing Manager, Content Strategist, Copy Editor, Marketing Communications Specialist
- **Company size:** 50–2,000 employees (typically companies with dedicated marketing functions)
- **Industries:** B2B SaaS, FinTech, Enterprise Software, Martech
- **Market size:** ~45,000 in-house content teams in North America; targeting companies with $5M–$1B ARR
- **Geographic scope:** Initially North America (US, Canada)

**Secondary Segment: Freelance and Agency Writers**

Individual freelancers and small agencies do similar work but with different workflows and constraints. We validate demand here but won't optimize for them in V1.

- **Job titles:** Freelance Copywriter, Content Agency Strategist, Content Consultant
- **Company size:** Solo operators to 20-person shops
- **Why secondary:** They often lack budget and move between projects; retention is harder. But they represent 15–20% of early adopters and provide valuable feedback.

---

### Problem Definition

**The Problem: Time Spent on Content Creation & Revision**

Today, content marketing teams spend an enormous amount of time on repetitive writing and revision tasks. A content marketing manager typically creates or oversees 8–15 pieces of content per month: blog posts, case studies, emails, product pages, ad copy, and social media content.

For a typical blog post (1,500–2,000 words), a content creator spends:
- 2–3 hours researching and outlining
- 2–4 hours drafting
- 1–2 hours revising for clarity and brand voice
- 30 minutes to 1 hour of editing/QA

**Total: 5.5–9.5 hours per piece.** For a team producing 40 pieces per quarter, that's 220–380 hours of labor annually on writing and revision alone. At an average marketing salary of $65,000/year ($31/hour fully loaded), that's **$6,800–$11,800 per person per year** spent just on content creation and editing.

**Current Solutions and Why They Fall Short**

Most teams use one of three approaches:

1. **Fully in-house creation:** Reliable for brand voice but slow and expensive. Requires hiring senior writers ($70K–$120K/year) or managing full-time content creators.

2. **Outsourced agencies:** Faster but expensive ($3,000–$8,000 per blog post) and requires weeks of revision cycles to match brand voice. Quality is inconsistent.

3. **Basic templates or AI tools (ChatGPT, generic assistants):** Fast but produces generic, off-brand content that requires heavy revision—often taking as long as writing from scratch. Teams report spending 2–3 hours revising AI output to match brand voice.

The core gap: **No tool lets teams generate quality, on-brand content quickly without extensive revision.**

---

### Validation Evidence

**Research Summary**

We conducted 12 in-depth interviews (45–75 minutes each) with content marketing managers and team leads between January–February 2025. All were from B2B SaaS companies with annual content budgets of $50K+.

**Key Findings:**

- **11 of 12 interviewees (92%)** confirmed that content creation speed and revision time are their top operational pain point
- **9 of 12 (75%)** said they currently use ChatGPT or similar tools but find the revision burden makes it barely faster than writing from scratch
- **10 of 12 (83%)** said they'd switch to a better solution if it reduced revision time by 50% or more
- **8 of 12 (67%)** indicated they'd be willing to pay $200–$500/month for a tool that reduced their team's content revision time

**Representative Quote from Interview #7 (Content Strategist at $500M SaaS company):**

> "We tried using ChatGPT to speed things up, but every piece still needs 2–3 hours of work to sound like us. It's not faster; it's just different work. If we could cut that revision time in half, we'd save a person-month of work per year. That's huge."

**Willingness to Pay**

Pricing model validation:
- 3 interviewees indicated $100–$200/month was too cheap (signaled skepticism about quality)
- 7 indicated $200–$500/month was fair value
- 2 indicated >$500/month was possible if ROI was clear ($1–1.5M teams with large content output)

**Competitive Analysis**

- Jasper AI, Copy.ai: Generic, no brand context; still require significant revision
- ChatGPT, Claude: Free or cheap but not designed for teams or brand management
- Grammarly: Editorial tool, not a content generator
- No direct competitor currently solves the "on-brand content generation at speed" problem

---

### User Context & Constraints

**Where and When Work Happens**

Content marketing teams typically work in asynchronous, distributed setups. A typical workflow:

1. Content strategist outlines topics in Slack or a shared doc
2. Writer drafts content in Google Docs or a CMS (often overnight or over 1–2 days)
3. Editor/manager reviews and comments, requesting revisions
4. Writer revises asynchronously (often in batches, not immediately)
5. Piece publishes to website, email, or social media

The process is fragmented across tools: Slack, Google Workspace, Hubspot, Notion, and email. Teams don't have a single "content hub" for AI-assisted work.

**Time Pressure and Deadlines**

Content calendars are planned monthly but often shift based on:
- Product launches (can happen with 2–3 weeks notice)
- Earnings calls or regulatory announcements
- Competitive moves
- Seasonal campaigns

Writers often face "I need this by end of week" pressure, especially for ad copy and email campaigns. This creates urgency around speed.

**Brand Voice and Consistency**

This is the highest-stakes constraint. Every company has a brand voice—formal vs. conversational, technical vs. accessible, humorous vs. serious. Large companies often have brand guidelines documents (20–50 pages). Current AI tools produce "generic corporate" output; adapting it to brand voice takes significant time.

Interviewees mentioned:
- Brand guidelines stored in Confluence or Google Drive (rarely searchable or well-indexed)
- Reliance on experienced writers who "just know" the voice
- Inconsistent output when junior writers or freelancers are involved

**Quality and Compliance Constraints**

- **B2B companies:** Content must be accurate, backed by data, and reflect company positioning
- **Regulated industries (FinTech, Healthcare):** Compliance review adds 1–2 weeks to publishing cycle
- **Legal review:** Enterprise deals often require legal sign-off on case studies and testimonials

---

### Success Criteria

If our product succeeds, we should see:

**Speed Metrics**
- Content creation time reduced from 5.5–9.5 hours to **2.5–4 hours per piece** (50% reduction)
- Revision cycles from 2–3 rounds down to **0–1 round** for well-scoped pieces
- Time-to-publish from 7–14 days to **3–5 days**

**Quality Metrics**
- Brand consistency score: 90%+ of AI-generated passages match brand voice in blind testing with team members
- Revision rate: <10% of initial AI drafts require substantial rewrites (vs. current 60–70% with generic AI)
- Accuracy: No factual errors introduced by AI (compliance-critical for regulated industries)

**Adoption Metrics**
- 60%+ of content created monthly uses the tool within first 6 months
- Average session time: 20–30 minutes (users spend time reviewing and editing, not fighting the interface)
- Team adoption: 70%+ of eligible content creators use the tool regularly

**Integration Requirements**
- Works seamlessly with existing CMS and publishing workflows (not another tab to flip between)
- One-click export to Google Docs, Hubspot, Notion
- Ability to input brand guidelines and update them as voice evolves

**User Confidence**
- Qualitative: "I trust this tool to maintain our brand" (vs. current skepticism of generic AI)
- Quantitative: 80%+ of users report increased confidence in output quality after 30 days

---

## Tips for Conducting User Research

**Talk to the right people, in depth.** 10–12 interviews with the right users (actual content creators and decision-makers) beats 50 shallow surveys. Go deep: understand their workflow, their tools, their constraints, and the specific language they use to describe problems.

**Watch for aspirational vs. real behavior.** Users will tell you they use certain tools or follow certain processes. Observe or ask detailed follow-up questions to understand what actually happens. ("How many hours do you spend revising AI output?—not the textbook answer, the real answer.")

**Map data requirements early.** Once you validate the problem, start asking: "What data would your tool need to understand your brand voice? How would you share it?" This reveals what kind of training data you'll need (brand guidelines, past writing samples, tone references) and informs your data collection and model fine-tuning strategy.

**Secondary research matters.** Interviews validate *who you're building for* and *why*, but market reports, industry benchmarks, and pricing research help you understand TAM and competitive positioning. Combine primary and secondary research for a complete picture.
