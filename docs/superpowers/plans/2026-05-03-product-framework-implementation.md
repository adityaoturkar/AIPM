# AI Product Framework Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Build and publish a complete AI Product Framework system with 5 templates, realistic examples, and professional GitHub presence.

**Architecture:** Create a structured set of reusable PM templates organized by workflow stage (Discovery → Strategy → Comms), with each template including instructions, blank template, and detailed realistic examples across 3 product scenarios (Writing Assistant, Search, Recommendation System).

**Tech Stack:** Markdown, Git, GitHub (public repository)

---

## File Structure

```
product-framework/
├── README.md                    # Root overview and navigation
├── discovery/
│   ├── user-research.md        # Problem validation framework
│   └── data-strategy.md        # Data requirements framework
├── strategy/
│   ├── model-requirements.md   # Model performance metrics framework
│   └── go-to-market.md         # Market positioning framework
└── comms/
    └── prd.md                  # Product requirements document framework
```

**Deliverable:** All files committed to git, pushed to GitHub, publicly accessible.

---

## Task 1: Initialize Repository Structure

**Files:**
- Create: `README.md` (placeholder)
- Create: `discovery/user-research.md` (will be filled in Task 2)
- Create: `discovery/data-strategy.md` (will be filled in Task 3)
- Create: `strategy/model-requirements.md` (will be filled in Task 4)
- Create: `strategy/go-to-market.md` (will be filled in Task 5)
- Create: `comms/prd.md` (will be filled in Task 6)

- [ ] **Step 1: Create folder structure**

```bash
mkdir -p discovery strategy comms
```

- [ ] **Step 2: Create placeholder files**

```bash
touch README.md
touch discovery/user-research.md
touch discovery/data-strategy.md
touch strategy/model-requirements.md
touch strategy/go-to-market.md
touch comms/prd.md
```

- [ ] **Step 3: Verify structure**

```bash
find . -type f -name "*.md" | sort
```

Expected output:
```
./README.md
./comms/prd.md
./discovery/data-strategy.md
./discovery/user-research.md
./strategy/go-to-market.md
./strategy/model-requirements.md
```

- [ ] **Step 4: Commit folder structure**

```bash
git add .
git commit -m "feat: initialize product framework folder structure"
```

---

## Task 2: Write User Research & Problem Validation Framework

**Files:**
- Create: `discovery/user-research.md`
- Example scenario: AI Writing Assistant

- [ ] **Step 1: Write user-research.md with complete content**

Create file at `discovery/user-research.md`:

```markdown
# User Research & Problem Validation

## Framework Overview

User Research is the foundation of AI product development. Before investing in model training or engineering, you need to validate that the problem you're solving is real, that users actually want the solution, and that your understanding of the user's context is accurate. For AI products specifically, this research informs both the problem definition AND the data you'll need to collect.

## When to Use

Conduct comprehensive user research at the start of a new product initiative or before entering a new market segment. This framework should guide your work for 2-4 weeks and inform everything downstream: your data strategy, model requirements, and go-to-market approach. You should have answers to these questions before you write the PRD.

## Key Sections (Blank Template)

### User Demographics & Segments
- Who are your target users? (job title, company size, industry)
- How many potential users? What's the addressable market?
- Are there sub-segments with different needs?

### Problem Definition
- What problem are they trying to solve?
- How do they currently solve it? (tools, workarounds, manual processes)
- What's the cost/pain of the current solution? (time, money, frustration)

### Validation Evidence
- How did you learn about this problem? (interviews, surveys, market research)
- How many users have you talked to? What's the quality of evidence?
- Is this a problem they actively seek solutions for, or something they tolerate?

### User Context & Constraints
- Where/when do they try to solve this problem?
- What tools or systems do they already use?
- What are the constraints? (time, budget, technical literacy, regulatory)

### Success Criteria
- How would they measure success? (speed, quality, cost savings, ease of use)
- What would make them switch from their current solution?
- What's the minimum viable solution they'd adopt?

---

## Realistic Example: AI Writing Assistant

### User Demographics & Segments

**Primary Segment: Content Marketing Teams**
- Users: Marketing managers, content creators, agency professionals
- Company size: Mid-market (50-500 employees) to large enterprises
- Industry: SaaS, agencies, publishing, e-commerce
- Market size: ~500K potential users globally; enterprise segment represents ~$2B TAM

**Secondary Segment: Individual Writers/Solopreneurs**
- Freelance writers, bloggers, independent consultants
- Less budget but higher volume; strong network effects potential
- Market size: ~5M potential users globally; lower revenue per user but high volume

### Problem Definition

Content creators spend 30-50% of their time on writing tasks that don't require creativity: drafting emails, writing product descriptions, creating social media captions, outlining blog posts. The current workflow is:
1. Stare at blank page (15+ minutes)
2. Write first draft manually (45+ minutes)
3. Edit and refine (30+ minutes)
4. Total: 1.5+ hours for a 500-word piece

Current solutions are fragmented: some use generic templates, some hire junior writers, some use basic grammar tools (Grammarly). None address the core problem: fast, high-quality content drafting at scale.

**Cost of current solution:** At $50/hour, one piece of content costs $75 in labor. A team producing 20 pieces/month spends $1,500/month on this work alone.

### Validation Evidence

Conducted 12 in-depth interviews with marketing managers and content creators (40 minutes each). Sample:
- 100% identified "fast, good-quality drafting" as their top pain point
- 85% currently use at least 2 different tools (templates, grammar checker, freelancer platforms)
- 67% said they'd pay $200-500/month for a solution that cut drafting time in half
- Interview feedback: "I spend more time formatting and reorganizing my thoughts than actually writing. If something could handle the skeleton, I'd focus on making it great."

Reviewed 8 competitor offerings (ChatGPT, Copy.ai, Jasper, etc.). Found that none focus specifically on team-based workflow or brand voice consistency—all are designed for one-off use.

Market research: Content marketing spend is growing 25%/year; agencies report hiring constraints as a blocker.

### User Context & Constraints

**Context:**
- Work happens in browser (Google Docs, Notion, marketing platforms)
- Often under time pressure ("need this by EOD")
- Collaborative: feedback from editors, managers, clients
- Brand voice consistency is critical (not generic writing)

**Constraints:**
- Content needs to reflect brand voice/guidelines (can't be generic)
- Some content is highly regulated (financial, healthcare)
- Quality bar is high (published content reflects brand)
- Data privacy concerns: some users can't upload proprietary content to third-party tools

### Success Criteria

Users would consider this successful if:
- **Speed:** 50% reduction in time spent on first draft (from 45 min to 22 min)
- **Quality:** Generated content requires <10% revision to meet publish standards
- **Integration:** Works within their existing workflow (Google Docs, Notion, Slack)
- **Brand consistency:** Output respects their brand voice/guidelines after light training

Minimum viable product they'd adopt: Tool that generates 3 draft options for a brief, any one of which they can finish in <10 minutes.

---

## Tips

- **Quality over quantity in interviews:** 8-12 deep interviews beat 100 surface-level surveys. You're looking for surprising insights, not validation.
- **Watch for aspirational vs. real behavior:** Users might say they'd pay premium prices, but actual behavior (switching costs, budget constraints) tells the real story. Test with actual willingness to pay, not hypotheticals.
- **Map data requirements early:** As you learn about user workflows, note what data you'd need to capture or train on. Example: if users care about brand voice, you need a way to quantify/learn brand voice (writing samples, guidelines, feedback loops).
- **Secondary research matters:** Competitive analysis, market research, and industry reports can validate demand and identify gaps. But no amount of secondary research replaces direct user evidence.
```

- [ ] **Step 2: Verify file content**

```bash
wc -w discovery/user-research.md
# Should be ~1,200 words
```

- [ ] **Step 3: Commit**

```bash
git add discovery/user-research.md
git commit -m "feat: write user research & problem validation framework"
```

---

## Task 3: Write Data Strategy Framework

**Files:**
- Create: `discovery/data-strategy.md`
- Example scenario: AI Search Product

- [ ] **Step 1: Write data-strategy.md with complete content**

Create file at `discovery/data-strategy.md`:

```markdown
# Data Strategy Framework

## Framework Overview

Data is the lifeblood of AI products. Your model is only as good as the data it's trained on. The Data Strategy framework forces you to think rigorously about what data you need, where you'll get it, how you'll maintain quality, and what it will cost. This is where many AI product teams fail—they optimize for model metrics without understanding the data pipeline and its limitations.

## When to Use

Develop your data strategy in parallel with User Research and before finalizing Model Requirements. You need to understand your users' problems well enough to know what data matters (from Task 2), and you need to validate that quality data is actually obtainable before you commit to model performance targets. Revisit this framework regularly as you learn more about data quality and availability.

## Key Sections (Blank Template)

### Data Required
- What data do you need to train the model? (text, images, structured data, user behavior)
- What's the minimum viable dataset size?
- How is quality defined for this data? (accuracy, recency, representativeness)

### Data Sources
- Where will you get this data? (user-generated, public datasets, synthetic, partnerships, crowdsourcing)
- Do you own the data or need licensing/permissions?
- What's the cost to acquire/maintain this data?

### Data Collection & Pipeline
- How will you collect data at scale? (automated, manual, user feedback loops)
- How often does data need to be refreshed?
- What's the pipeline for storing, labeling, versioning?

### Data Quality & Bias
- How will you ensure quality? (validation metrics, human review, automated checks)
- What biases might exist in your data? (demographic, geographical, temporal)
- How will you audit and mitigate bias?

### Data Privacy & Compliance
- What regulations apply? (GDPR, CCPA, industry-specific)
- How will you handle PII and sensitive data?
- What's the user consent/data usage policy?

### Data Costs
- What's the cost to acquire/label/maintain data per unit?
- How does this scale with model performance improvements?
- What's the ROI on data collection vs. alternative approaches?

---

## Realistic Example: AI Search Product

### Data Required

A semantic search product needs two distinct datasets:

**1. Indexing Data (corpus to search over)**
- Document corpus: 500M+ documents (internal knowledge bases, PDFs, web content)
- Metadata: document title, source, last updated, access permissions
- Quality bar: Content should be recent (not >2 years old except for reference material) and relevant to search intent

**2. Training Data (for relevance ranking)**
- Query-document pairs with relevance labels: 100K+ labeled examples
- Quality bar: High precision on relevance judgments (>95% inter-rater agreement)

### Data Sources

**Indexing data:**
- Primary: User-provided documents (enterprise clients upload their own content)
- Secondary: Public datasets (Common Crawl for initial MVP), partnerships
- Estimated cost: Free if user-provided; $50K-100K for 1M public documents

**Training data:**
- Domain experts to label relevance: 20-40 contractors ($8K-12K project cost)
- User feedback loops: Track which search results users click on, which they skip (signals relevance)
- Estimated cost: $15K upfront; ongoing is essentially free once user feedback loop is live

### Data Collection & Pipeline

**Phase 1 (MVP, Month 1-2):**
- Manual labeling: 5 domain experts label 10K query-document pairs over 2 weeks
- Automated validation: Automatic check that labels are consistent, no obvious errors
- Storage: Simple CSV files in S3, versioned with timestamps

**Phase 2 (Scale, Month 3+):**
- User feedback loop: Track all queries, user clicks, dwells, skips
- Weekly data refresh: Incorporate new user queries and feedback into training set
- Automated quality checks: Detect label inconsistencies, alert on data drift

**Pipeline architecture:**
```
User queries + document corpus
    ↓
[Semantic embedding]
    ↓
[Ranking model]
    ↓
[User click feedback]
    ↓
[Retrain weekly]
```

### Data Quality & Bias

**Quality assurance:**
- 10% of labels reviewed by secondary expert; flag disagreements >20%
- Monthly audit: Sample 100 queries, manually judge search results (gold standard)
- Automated checks: Reject labels with extremely high/low confidence

**Potential biases:**
- Selection bias: Training queries are skewed toward popular topics; rare queries underrepresented
- Labeler bias: Domain experts may have their own ranking preferences (e.g., prefer academic sources)
- Temporal bias: If indexing stale documents, model learns to rank old results highly

**Mitigation:**
- Regularly sample queries from tail (low-frequency queries); label separately to weight higher
- Use multiple labelers; weight labels inversely by labeler agreement (uncertain labels weighted less)
- Actively monitor result quality on diverse queries; retrain often to avoid staleness

### Data Privacy & Compliance

**GDPR/CCPA considerations:**
- Users can request data deletion (remove their documents from index)
- Anonymize search queries after 90 days (don't store PII in query logs)
- Document data retention policy: Training data kept 1 year; search logs kept 3 months

**Enterprise compliance:**
- SOC 2 compliance required; data encrypted at rest and in transit
- Customers can keep documents on-premise with API integration (not all data goes to our servers)
- Clear data usage terms: search logs used only to improve ranking, not for other purposes

### Data Costs

**Acquisition/labeling:**
- Labeling cost per query-document pair: $0.15-0.30 (expert review)
- 100K labeled pairs: $15K-30K (one-time)
- Per 10K new labels/month: $1,500-3,000

**Maintenance:**
- Storage: $2-5K/month for 500M documents
- Data refresh/validation: $3-5K/month (automated checks + quarterly audits)
- Total data cost: ~$7-8K/month

**ROI calculation:**
If your search product is enterprise SaaS at $1K/month per customer, you need 8-12 customers just to cover data costs. After that, data cost is <1% of revenue.

---

## Tips

- **User-generated data is most valuable:** If your product can turn user behavior into training signal (clicks, feedback, corrections), you unlock a virtuous cycle where the product gets better as it's used. Plan your data pipeline around this from day one.
- **Quality beats quantity:** 10K high-quality labeled examples beat 100K noisy examples. Invest in labeling quality, not just volume.
- **Test assumptions about data availability:** Before you commit to a model architecture, run a small labeling experiment (100-500 examples). Can you achieve consistent labels? How long does it take? Does the data exist?
- **Data cost is often underestimated:** Collection, labeling, validation, compliance, and privacy all cost more than you think. Build this into your financial model early.
```

- [ ] **Step 2: Verify file content**

```bash
wc -w discovery/data-strategy.md
# Should be ~1,300 words
```

- [ ] **Step 3: Commit**

```bash
git add discovery/data-strategy.md
git commit -m "feat: write data strategy framework"
```

---

## Task 4: Write Model/Performance Requirements Framework

**Files:**
- Create: `strategy/model-requirements.md`
- Example scenario: AI Recommendation System

- [ ] **Step 1: Write model-requirements.md with complete content**

Create file at `strategy/model-requirements.md`:

```markdown
# Model & Performance Requirements Framework

## Framework Overview

Model requirements define what "success" means for your AI system. Unlike traditional software where success is binary (works or doesn't), AI systems operate in shades of gray. You need to define the metrics that matter for your users and business, the performance thresholds you need to hit, and the trade-offs you're willing to make. This framework ensures your model optimization is aligned with real product goals, not just research metrics.

## When to Use

Develop Model Requirements in parallel with Data Strategy and after completing User Research. You'll reference this framework when evaluating model architectures, prioritizing which features to build, and deciding when the model is "good enough" to ship. Revisit quarterly as you gather real performance data.

## Key Sections (Blank Template)

### Success Metrics
- What metrics will you use to measure model performance? (accuracy, precision, recall, F1, NDCG, AUC, etc.)
- Why do these metrics matter to users/business?
- What are the target thresholds? (e.g., >95% precision, <100ms latency)

### Business Metrics
- How does model performance translate to user satisfaction? (engagement, retention, revenue)
- What's the relationship between model accuracy and business outcome?
- Example: 1% improvement in recommendation CTR = $X revenue impact

### Baseline & Comparisons
- What's your baseline? (existing product, simple heuristics, competitor)
- What performance would beat the baseline? By how much?
- What's the performance of competing solutions?

### Performance Trade-offs
- Speed vs. accuracy: How fast must the model run? What accuracy are you willing to sacrifice for speed?
- False positives vs. false negatives: Which type of error costs more?
- Coverage vs. quality: How many requests can you handle? What's acceptable fallback behavior?

### Fairness & Bias Metrics
- How will you measure fairness across user segments? (demographic parity, equal opportunity)
- What's acceptable disparity between segments? (e.g., <5% difference in performance)
- How will you audit and monitor bias in production?

### Success Criteria & Acceptance Thresholds
- At what point is the model good enough to ship to beta users?
- At what point can you roll out 100%?
- What hard constraints (latency, cost) must be met?

---

## Realistic Example: AI Recommendation System

### Success Metrics

For a recommendation system, there are three layers of metrics:

**1. Ranking Metrics (what the algorithm optimizes)**
- Click-Through Rate (CTR): % of recommendations that users click
- Conversion Rate: % of clicks that lead to purchase/engagement
- NDCG (Normalized Discounted Cumulative Gain): Quality of ranking at positions 1-5 (position 1 worth more than position 5)
- Diversity: % of recommendations from different categories (avoid recommending the same type repeatedly)

**2. User Satisfaction Metrics (how users perceive it)**
- Satisfaction survey: "Did you find useful recommendations?" (5-point scale)
- Serendipity: "Did you discover something you wouldn't have found otherwise?" (yes/no)
- Engagement: Time spent, return frequency, recommendation acceptance rate

**3. Business Metrics (impact on P&L)**
- Revenue per user (impact of recommendations on purchase value)
- Retention (do recommendations improve user stickiness?)
- Operational cost (infrastructure, inference latency)

### Business Metrics

**Relationship between model performance and business outcome:**

- **Baseline:** Without recommendations, 5% of users make purchases; avg order value $50. Revenue per user: $2.50/month
- **Target:** With strong recommendations, goal is 10% conversion on recommended items; avg recommendation-influenced order value: $75
- **Expected impact:** 5% increase in conversion → +$2.50 revenue per user per month → $2.5M incremental annual revenue (with 100K users)

**Why this matters:** An improvement in NDCG from 0.65 to 0.72 is meaningless on its own. But if that improvement correlates with a 2% increase in recommendation acceptance, that's worth ~$500K/year. Now you have a business reason to invest engineering effort.

### Baseline & Comparisons

**Baseline (existing recommendation approach):**
- Simple collaborative filtering: "users who bought X also bought Y"
- Performance: CTR 3%, diversity 40% (mostly recommending best sellers)
- Latency: 50ms per request
- Cost: $5K/month infrastructure

**Target performance (your system):**
- ML-based personalization: Deep learning model trained on user behavior + content features
- Target: CTR 6-8%, diversity 70%, latency <100ms, cost <$8K/month
- Success threshold: Must beat baseline by 2x+ on CTR while maintaining lower cost

**Competitor benchmarks:**
- Amazon recommendations: 20-30% CTR (but massive data advantage, different domain)
- Spotify: 8-12% skip rate on algorithmic playlists (our analog: 92-88% acceptance)
- Realistic expectation for us: 5-7% CTR is very strong for our domain; 8%+ would be exceptional

### Performance Trade-offs

**Speed vs. Accuracy:**
- Real-time constraint: Must respond in <100ms (user won't wait longer)
- Accuracy trade-off: Simpler model = faster but less accurate. Need to find the sweet spot
- Decision: Use ensemble of 2-3 models in parallel; return best result that arrives within 100ms

**False positives vs. false negatives:**
- False positive: Recommend something user doesn't like (wastes their time)
- False negative: Don't recommend something user would have loved (lose engagement)
- We care more about false negatives (missing a good rec is worse than one bad rec among 5)
- Threshold decision: Use 0.3 confidence threshold for recommendations (only show if >30% sure user will like it)

**Coverage vs. Quality:**
- Coverage: Can you make recommendations for all users? (New users, niche interests)
- Quality: How good are recommendations when you have limited data?
- Decision: For new users (cold-start), use content-based + popularity fallback; quality will be lower but coverage 100%

### Fairness & Bias Metrics

**Measuring fairness across segments:**
- Demographic: Do male/female users get equally good recommendations? → Monitor CTR by gender
- Geographic: Do US/international users experience different quality? → Monitor CTR by region
- User tenure: Do new users get worse recommendations? → Monitor CTR for users <30 days, 30-90 days, >90 days

**Acceptable disparity:**
- Hard constraint: No segment should have >5% lower CTR than average
- If we detect >5% disparity, treat as bug and prioritize fix
- Monthly audit: Slice performance by all dimensions, alert on new disparities

**Monitoring bias in production:**
- Weekly report: CTR/satisfaction metrics by segment
- Automated alerts: If any segment drops >3% week-over-week, alert on-call
- Quarterly deep dives: Analyze why certain segments underperform; collect user feedback

### Success Criteria & Acceptance Thresholds

**MVP (Beta with 5% of users):**
- Minimum: CTR >4%, latency <150ms, no critical fairness issues (>10% disparity)
- Recommendation: Wait for CTR >5%, latency <100ms, all segments within 5%

**Limited rollout (25% of users):**
- Requirement: CTR >5.5%, all segments >5% disparity, <5 customer complaints per 10K users about rec quality
- Success criterion: Revenue impact detectable (>0.5% increase in conversion)

**Full rollout (100% of users):**
- Requirement: CTR >6%, all segments within 3% disparity, <2 complaints per 10K users
- Hard constraint: Must maintain sub-100ms latency, system cost must stay <$10K/month

**Continuous improvement targets (post-launch):**
- Month 3: 6.5% CTR
- Month 6: 7% CTR
- Month 12: 7.5% CTR

---

## Tips

- **Connect metrics to user experience:** "NDCG improved from 0.68 to 0.71" means nothing to users. "Recommendations users click on increased from 4% to 5%" means something. Link technical metrics to user-facing outcomes.
- **Beware of metric gaming:** If you optimize only for CTR, models will recommend clickbait. Define multiple metrics and weight them together so the model can't game a single metric.
- **Real-world performance != test set performance:** Your model might hit 95% accuracy on a test set but 60% in production because production data is different (concept drift, new user types, seasonality). Plan for this gap.
- **Fairness is not optional:** Biased recommendations destroy user trust. Make fairness metrics as important as accuracy metrics from day one; don't patch it in later.
```

- [ ] **Step 2: Verify file content**

```bash
wc -w strategy/model-requirements.md
# Should be ~1,300 words
```

- [ ] **Step 3: Commit**

```bash
git add strategy/model-requirements.md
git commit -m "feat: write model & performance requirements framework"
```

---

## Task 5: Write Go-to-Market & Positioning Framework

**Files:**
- Create: `strategy/go-to-market.md`
- Example scenario: AI Writing Assistant

- [ ] **Step 1: Write go-to-market.md with complete content**

Create file at `strategy/go-to-market.md`:

```markdown
# Go-to-Market & Positioning Framework

## Framework Overview

Building a great product is only half the battle. How you position it, who you sell to first, and how you communicate its value determine whether anyone will actually use it. For AI products specifically, positioning is even more critical because users have high expectations and skepticism about AI capabilities. You need to be clear about what the AI actually does vs. what users hope it will do, and why your solution beats existing alternatives.

## When to Use

Develop your GTM strategy in parallel with Model Requirements, after you've validated the problem and understand what your product can actually deliver. Revisit this framework every quarter as your product capabilities evolve and you learn about competitive threats.

## Key Sections (Blank Template)

### Target Customer
- Who is your ideal customer? (size, industry, role, budget)
- Why are they best-suited to benefit from your product?
- What are their specific use cases / pain points?

### Value Proposition
- What is the core benefit your product delivers? (speed, quality, cost savings, new capability)
- How is this different from alternatives? (incumbents, DIY, competitors)
- What's the one sentence that captures why someone should care?

### Positioning Statement
- How do you want to be perceived in the market?
- Are you the "premium/best quality" or "affordable/accessible" option?
- What is the single most important differentiator?

### Competitive Landscape
- Who are your direct competitors? (other AI solutions, existing workflows)
- What do they do well? What are their weaknesses?
- Why will customers choose you over them?

### Go-to-Market Strategy
- How will you reach customers? (sales, self-serve, partnerships, viral)
- What's your pricing model? (freemium, SaaS, per-use, enterprise)
- What's your launch plan? (beta, limited launch, full launch)

### Customer Acquisition & Economics
- What channels will drive customer acquisition?
- What's the cost to acquire a customer? (CAC)
- What's the lifetime value? (LTV)
- Is the CAC:LTV ratio profitable?

### Messaging & Communication
- What's the core message for different audiences? (users, managers, investors)
- What are the top 3 benefits you emphasize?
- What objections will you encounter? How do you address them?

---

## Realistic Example: AI Writing Assistant

### Target Customer

**Primary:** Content marketing managers at B2B SaaS companies (Series A - Series C)
- Company size: 50-500 employees
- Marketing team size: 3-15 people
- Annual marketing budget: $500K-5M
- Pain: Scaling content production (blog, emails, social, case studies) without hiring more writers

**Why this segment:**
- High budget to pay for tools ($200-500/month per user)
- Concrete metric for success (output quantity + quality)
- Existing workflows where our tool integrates (Google Docs, Notion, marketing platforms)
- Network effects: If we win one company, often win their entire team

**Specific use cases:**
- Marketing managers: Drafting blog outlines, social media captions, email campaigns
- Account executives: Writing personalized outreach, case study summaries
- Product managers: Writing release notes, feature announcements

### Value Proposition

**Core benefit:** Reduce time to first draft by 50% while maintaining brand voice and quality.

**Why this matters:** Saves 5-10 hours/week per marketer; at $75/hour, that's $375-750/week = $19.5K-39K/year saved per employee.

**How we're different:**
- **vs. ChatGPT:** ChatGPT is generic and requires prompting expertise; we're tuned for brand voice and marketing workflows
- **vs. Copy.ai:** Copy.ai generates lots of options but low quality; we focus on fewer, higher-quality drafts
- **vs. Hiring:** Hiring writers takes 2-3 months, costs $50K+/year; we're immediate and scalable

**One-sentence pitch:** "An AI writing tool built specifically for marketing teams that learns your brand voice and cuts drafting time in half."

### Positioning Statement

Position as the "professional writer's assistant" not the "AI replacement for writers."

**Positioning narrative:**
- **We're not:** A replacement for human writers, a generic content generator, another ChatGPT wrapper
- **We are:** A productivity tool that handles the tedious 30-40% of writing (outlining, first drafts) so humans focus on the creative 60-70% (refining, brand voice, strategy)
- **Why it matters:** Companies want better content faster, but won't trust AI to write it alone. We're the co-pilot, not the pilot.

**Proof:** Show examples of raw AI output + human-refined version. Prove the thesis that a human + AI produces better work in less time than either alone.

### Competitive Landscape

**Direct competitors:**
- ChatGPT: Stronger model, worse UX for workflows, no brand voice learning, no integrations
  - Why we win: Better integrated, faster for specific use cases, more reliable output
- Copy.ai: Purpose-built for marketing, but generates 10+ low-quality options
  - Why we win: Fewer, higher-quality drafts; better for brand voice
- Jasper: Enterprise-grade, high price ($125+/month)
  - Why we win: Simpler, cheaper ($29-99/month), easier to use

**Indirect competitors:**
- Hiring freelancers: Takes weeks, costs 3x as much, harder to manage
- Internal hire: Takes months, costs $50K+/year, still needs editors
- DIY with templates: Time-consuming, lower quality, still requires human effort

**Why customers choose us:**
- Speed: Get drafts in minutes, not hours or weeks
- Quality: Output needs <10% revision vs. 20-30% for generic tools
- Accessibility: Easier to use than ChatGPT; more affordable than hiring

### Go-to-Market Strategy

**Phase 1 (Months 1-3): Beta with hand-picked customers**
- Target: 20-30 early users from target segment
- Channel: Direct outreach to content-forward startups (warm intros, Product Hunt, content marketing communities)
- Model: Free beta in exchange for feedback
- Goal: Validate product-market fit, get testimonials, refine positioning

**Phase 2 (Months 4-6): Controlled launch**
- Target: 200-500 users
- Channel: Content marketing blog + SEO, ProductHunt, early adopter communities (IndieHackers, MicroConf)
- Pricing: $29/month for starter, $99/month for teams
- Goal: Achieve 20%+ monthly user growth, 50%+ retention

**Phase 3 (Months 7+): Scale with partnerships**
- Target: Expand to agencies, in-house teams
- Channel: Partnerships with CMS platforms (Webflow, WordPress plugins), email tools (Convertkit), design tools (Figma)
- Pricing: Same tiers + enterprise plans at $500+/month for features + integrations

### Customer Acquisition & Economics

**Phase 1 (Beta):**
- CAC: $0 (organic, referrals)
- LTV: N/A (free product)

**Phase 2 (Paid tier):**
- Channels: 40% content/SEO, 30% product communities, 20% partnerships, 10% paid ads
- CAC: ~$50 (organic content is cheaper; paid ads ~$100 CAC)
- LTV: $1,200 (assuming $50 ARPU, 24-month retention)
- CAC:LTV: 1:24 ✓ (healthy)

**Expansion opportunity:**
- Starter users ($29/month) convert to Team plan ($99/month) at 15% rate
- Blended ARPU after expansion: $50 → $65
- LTV: $1,560
- CAC:LTV: 1:31 (very healthy)

### Messaging & Communication

**For individual writers/marketers:**
- Lead: "Cut your drafting time in half"
- Supporting: "Maintains your brand voice, integrates with your workflow, built by marketers for marketers"
- CTA: "Try free for 7 days"

**For marketing managers/leadership:**
- Lead: "Scale content production without scaling headcount"
- Supporting: "50% faster drafts, maintains quality, $X savings per team member per year"
- CTA: "Schedule a 15-min demo"

**For investors/partners:**
- Lead: "AI writing assistant for the $200B content marketing market"
- Supporting: "$1.5B+ TAM, strong product-market fit in B2B SaaS, $X MRR with Y% MoM growth"
- CTA: "Funding inquiry / partnership exploration"

**Common objections & responses:**
- "The output is generic / not good enough": Show before/after examples; emphasize it's a co-pilot not a replacement
- "We use ChatGPT, why not free?": ChatGPT requires prompting expertise; we're optimized for your workflow and brand
- "We're not sure the quality will match our standards": Free trial period; testimonials from similar companies; money-back guarantee
- "Privacy concerns with AI tools": Data is encrypted, never used to train other models, can be deleted on request

---

## Tips

- **Positioning is not features:** Don't list 10 features. Pick the single most important benefit for your customer and lead with that. Everything else supports that claim.
- **Know thy enemy:** You don't need to beat everyone. But you need to beat the specific alternative your customer would choose if you didn't exist (which might be "do nothing manually").
- **CAC:LTV needs to be >1:3 for SaaS viability:** If you're spending $100 to acquire a customer worth $100 lifetime, you won't survive. Aim for 1:5+ and you can scale.
- **Messaging evolves with traction:** Your first positioning might be wrong. As you gain users, pay attention to what actually resonates (who buys, how they describe it, why they switch from alternatives). Your messaging in Month 6 will be different (and better) than Month 1.
```

- [ ] **Step 2: Verify file content**

```bash
wc -w strategy/go-to-market.md
# Should be ~1,300 words
```

- [ ] **Step 3: Commit**

```bash
git add strategy/go-to-market.md
git commit -m "feat: write go-to-market & positioning framework"
```

---

## Task 6: Write PRD (Product Requirements Document) Framework

**Files:**
- Create: `comms/prd.md`
- Example scenario: AI Search Product

- [ ] **Step 1: Write prd.md with complete content**

Create file at `comms/prd.md`:

```markdown
# Product Requirements Document (PRD) Framework

## Framework Overview

A PRD is the canonical source of truth for what you're building and why. It's the artifact you share with engineers, designers, stakeholders, and investors to ensure everyone understands the same thing. A good PRD is clear enough that an engineer can build from it, detailed enough that edge cases are thought through, but concise enough that someone can skim it in 15 minutes and understand the core idea. For AI products, PRDs need to be especially careful about defining model behavior, failure cases, and user expectations around AI limitations.

## When to Use

Write the PRD after you've completed User Research, validated that the problem is real, and agreed on Model Requirements. The PRD documents the decisions made in those earlier frameworks. Update it as you learn more during development, but treat it as a stable artifact—major changes should be tracked and discussed, not silently rewritten.

## Key Sections (Blank Template)

### Executive Summary
- Problem statement: What problem are you solving?
- Solution: How do you solve it in one sentence?
- Impact: What's the expected user/business impact?

### Goals & Success Metrics
- What does success look like? (user engagement, business metrics, model performance)
- What are the acceptance criteria?
- How will you measure success?

### User Stories / Use Cases
- Who are the users?
- What do they want to do?
- Why do they want to do it?
- Acceptance criteria for each use case

### Product Requirements
- What features does the product include?
- What are the exact specifications? (inputs, outputs, behavior)
- What are the edge cases / error handling?

### User Experience & Workflows
- How does the user interact with the product?
- What's the happy path?
- What happens when things go wrong?

### Technical Approach
- What's your architecture/approach?
- Why this approach over alternatives?
- What are the key technical decisions and trade-offs?

### Risks & Mitigations
- What could go wrong?
- How will you mitigate each risk?
- What's the fallback plan?

### Timeline & Scope
- What's in scope for v1.0?
- What's explicitly out of scope?
- What's the timeline?

---

## Realistic Example: AI Search Product

### Executive Summary

**Problem statement:** Enterprise teams spend 15+ minutes per day searching through internal documents, wikis, Slack, and emails trying to find information. Current tools (Slack search, Jira search, Gmail search) are keyword-based and fragile—you have to know exactly what to search for, or you get nothing.

**Solution:** An AI-powered semantic search engine that understands what users are looking for, even when they don't use the exact keywords. Users type a question in natural language and get relevant documents ranked by usefulness.

**Impact:** Reduce time spent searching by 50% (from 15 min to 7.5 min per day); increase information discovery (users find answers they wouldn't have found with keyword search); improve decision-making (better information access).

### Goals & Success Metrics

**User goals:**
- Find relevant documents in <30 seconds
- Get useful results even with vague queries
- Understand why results are ranked that way

**Business goals:**
- Drive 10% of enterprise customers to adopt paid search tier
- Increase NPS by 15 points (from 45 → 60) by solving a major pain point
- Reduce support burden (fewer "where can I find X?" questions)

**Product metrics (success criteria):**
- CTR (click-through rate) on search results >6% (beat baseline of 3%)
- Relevance score (users rating results useful) >75%
- NDCG@5 >0.75 (quality of top 5 results is high)
- Latency <100ms (returns results faster than user can drink coffee)
- Zero critical failures (search should always return something, never error out)

### User Stories / Use Cases

**Use Case 1: Searching for a past discussion**

User: Slack power user who needs to reference a conversation from 3 months ago

Query: "How did we decide to prioritize the API work?"

Expected behavior:
- System understands "prioritize" even if the original Slack message said "decide on roadmap"
- Returns top 3-5 Slack threads that discuss API prioritization
- User can click to jump to that thread in Slack
- Acceptance criteria: Must return relevant result within 2 clicks, <50ms latency

**Use Case 2: Researching a topic across documents**

User: Product manager preparing for a roadmap review, needs context on current state

Query: "What's our current strategy for mobile?"

Expected behavior:
- System searches across all documents (Slack, Jira, Notion, Google Docs, emails)
- Returns relevant docs ranked by recency and relevance
- Shows snippets so user can preview without opening each doc
- Acceptance criteria: Top result is relevant 80%+ of the time, all results from last 2 years

**Use Case 3: Troubleshooting a technical issue**

User: Engineer debugging a production issue, needs to find past incident reports or documentation

Query: "Payment processing failures intermittent timeout"

Expected behavior:
- System surfaces past incident reports, runbooks, code comments with relevant context
- Distinguishes between "timeout as a symptom" vs. "timeout as a solution"
- Returns actionable results (runbooks, fixes) ranked higher than generic docs
- Acceptance criteria: First result is actionable 90% of the time

### Product Requirements

**Core feature: Semantic search**

Input:
- Query: Free-text natural language (50-500 characters)
- Scope: User can optionally filter by document type (Slack, Jira, Email, Docs)
- Source data: All documents the user has access to (respects existing permissions)

Output:
- Top 10 results ranked by relevance
- For each result: Title, snippet (preview), source (Slack, Jira, Doc name), timestamp
- Relevance explanation: Why was this result returned? (optional, helps user understand)

Behavior:
- If query is too short (<3 characters): Show trending searches instead
- If no results found: Suggest related searches; don't error out
- If permission denies access: Hide those results; don't surface to user

**Secondary features:**
- Saved searches: Users can save frequent queries for quick re-run
- Search filters: Filter by date range, document type, author
- Search history: Last 20 queries available in sidebar

**What's NOT included (out of scope):**
- Boolean search operators (AND, OR, NOT) — we're doing semantic, not keyword-based
- Search result explanations (why was this ranked first?) — complexity, latency concerns
- Real-time indexing of new Slack messages — we index hourly, acceptable lag
- Multi-language support — English only for v1

### User Experience & Workflows

**Happy path:**

```
1. User opens search interface (Slack bot, email, or web app)
2. Types query: "latest OKRs for Q4"
3. System returns 10 results within 100ms
4. User clicks result (Jira ticket "Q4 OKRs")
5. Jump to that document with context highlighted
```

**Edge case: Ambiguous query**

```
1. User types: "project status" (ambiguous—could mean many things)
2. System returns top 10 results across different projects
3. User sees results and realizes "oh, they meant Project X"
4. User refines query: "Project X status"
5. System returns more specific results
```

**Error case: Permission denied**

```
1. User searches for "compensation framework" (exists, but user doesn't have access)
2. System doesn't return those results
3. System shows: "No results found. Tip: If you think results are being hidden, contact your admin."
4. User isn't confused about why they found nothing
```

### Technical Approach

**Architecture:**
```
New documents (Slack, Jira, Docs, Email)
    ↓
[Extract + Chunk documents]
    ↓
[Embed chunks with semantic model (e.g., OpenAI embeddings or open-source)]
    ↓
[Store in vector database (Pinecone, Weaviate, Milvus)]
    ↓
[User query comes in]
    ↓
[Embed query with same model]
    ↓
[Semantic search in vector DB: find most similar embeddings]
    ↓
[Re-rank results with ML ranking model (LambdaMART, learned-to-rank)]
    ↓
[Return top 10 + snippets]
```

**Why this approach:**
- Semantic embedding captures meaning, not just keywords
- Vector database scales to millions of documents
- Re-ranking allows us to incorporate signals beyond similarity (recency, engagement, authority)
- OpenAI embeddings start: high quality, no training required; can migrate to open-source later

**Key technical decisions:**

1. **Embedding model:** Start with OpenAI text-embedding-3-small (cheap, good quality); migrate to open-source when performance allows
2. **Vector database:** Use Pinecone (managed, no ops overhead) vs. self-hosted Milvus (cheaper at scale, but requires ops)
3. **Re-ranking:** Start simple (BM25 + recency); add ML re-ranker only if CTR not hitting targets
4. **Indexing:** Batch index every hour; good enough for 99% of use cases

### Risks & Mitigations

| Risk | Impact | Mitigation |
|------|--------|-----------|
| Embedding model is low quality; irrelevant results | Users stop using product, NPS drops | A/B test embedding models early; have fallback to keyword search |
| Latency >500ms; users see slow search | Hurts engagement; users don't use feature | Optimize vector DB queries; cache popular queries; use simpler model if needed |
| Privacy: user A sees user B's documents | Data breach, legal liability | Enforce access control at query time; regularly audit for leaks; encrypt data at rest |
| Bias: search favors certain document types | Users get worse results; lower adoption | Monitor CTR by document type; retrain model if disparity >10% |
| Scale: index grows to 1B+ documents | Query latency increases; cost balloons | Use approximate nearest neighbor (ANN); shard by team/customer; migrate to self-hosted if needed |

### Timeline & Scope

**v1.0 (MVP, 6 weeks):**
- Scope: Search Slack, Jira, Google Drive documents
- Features: Basic semantic search, filters by date/type, 10 results
- Success: CTR >5%, latency <150ms, 50+ beta customers with 20%+ weekly active
- Out of scope: Email/chat integration, re-ranking, saved searches, multi-language

**v1.1 (8 weeks after v1):**
- Scope: Email integration, re-ranking with ML model, saved searches
- Success: CTR >6%, NDCG@5 >0.75

**v2.0 (6 months+):**
- Scope: Multi-language, real-time indexing, explanation for results, API for integrations

---

## Tips

- **PRD is not design:** Don't describe the UI in pixel-level detail. Describe the behavior and requirements; let designers figure out the UI.
- **Acceptance criteria must be testable:** "Easy to use" is not testable. "CTR >6%" is testable. "Latency <100ms" is testable. Write requirements you can actually verify.
- **Edge cases are where most bugs live:** Spend time thinking about what happens when things go wrong. Low query volume? Permission denied? Network failure? Model confidence is low? These edge cases matter.
- **AI products need extra clarity on failure modes:** Users expect determinism from software, but AI is probabilistic. Be explicit: "Results may not be perfect. If you can't find what you need, try rephrasing your query." This sets expectations and builds trust.
```

- [ ] **Step 2: Verify file content**

```bash
wc -w comms/prd.md
# Should be ~1,500 words
```

- [ ] **Step 3: Commit**

```bash
git add comms/prd.md
git commit -m "feat: write PRD framework"
```

---

## Task 7: Write Root README.md

**Files:**
- Create: `README.md` (root)

- [ ] **Step 1: Write comprehensive README.md**

Create file at `README.md`:

```markdown
# Product Framework

A comprehensive PM methodology and template system for building AI products. This framework walks through the complete product development cycle—from problem discovery through market launch—with practical templates and detailed examples.

## What Is This?

This is not a generic PM toolkit. These are the frameworks and templates I use for thinking about AI products specifically. AI products have unique challenges: uncertainty about model capabilities, the importance of data quality and bias, the need to manage user expectations around AI limitations. This framework addresses those challenges directly.

Use this repository to:
- **Learn my PM approach:** How I think about product decisions in AI/ML contexts
- **Prepare for interviews:** Reference these templates when discussing your product philosophy
- **Apply to your own work:** Adapt these frameworks for your AI product projects
- **Understand the full cycle:** See how research, data strategy, and model requirements connect

## The Five Frameworks

| Framework | Stage | Purpose | Key Questions |
|-----------|-------|---------|----------------|
| **User Research & Problem Validation** | Discovery | Validate the problem is real before you build | Who has the problem? How bad is it? Are they willing to solve it? |
| **Data Strategy** | Discovery | Plan your data pipeline and address data challenges | What data do you need? Where will you get it? How will you ensure quality? |
| **Model & Performance Requirements** | Strategy | Define what "good enough" means for your model | What metrics matter? What performance targets will you hit? |
| **Go-to-Market & Positioning** | Strategy | Plan how you'll win in the market | Who should you target first? How are you different? How will you acquire customers? |
| **PRD (Product Requirements Document)** | Comms | Communicate the complete product vision clearly | What are you building? How does it work? What's in/out of scope? |

## How to Use This Repository

**For learning:** Start with `/discovery` if you want to understand problem validation and data thinking. Move to `/strategy` for model planning and market positioning. `/comms` shows how to synthesize everything into a coherent product plan.

**For your own projects:** Treat each `.md` file as a template. Copy the "Key Sections" into a new document. Fill in your own examples (real or hypothetical). The blank template is meant to guide your thinking, not to be prescriptive.

**For interviews:** Reference specific frameworks and examples to discuss how you approach product decisions. Example: "When I was thinking about [product], I used the Data Strategy framework to identify that [decision]."

## The Three Product Scenarios

Each framework includes a detailed, realistic example. To show versatility, examples are drawn from three different AI product scenarios:

1. **AI Writing Assistant** — Content quality, model evaluation, brand voice
2. **AI Search Product** — Retrieval, ranking, user behavior signals
3. **AI Recommendation System** — Personalization, cold-start problems, A/B testing

This variety shows that the same frameworks apply across different AI product types.

## What Makes These Frameworks AI-Specific?

1. **Emphasis on data as a product input:** Unlike traditional software, AI product quality is directly tied to data quality. Every framework addresses data implications.

2. **Model metrics vs. business metrics:** The gap between "good accuracy on a benchmark" and "users actually find this useful" is large. These frameworks help you bridge that gap.

3. **Failure mode thinking:** AI systems fail differently than traditional software. These frameworks include planning for ambiguity, bias, and edge cases.

4. **Expectation setting:** AI products need to be clear about what they can and can't do. These frameworks help you communicate limitations without losing user trust.

## How to Contribute

This is a personal framework—it reflects my approach and thinking. If you find issues or have suggestions, issues and PRs are welcome. But understand that this is not a community-driven toolkit; I'm not trying to build the "ultimate" PM framework. This is how I think, shared publicly in case it's useful to you.

## License

These templates and frameworks are shared freely. Use them for learning, interviews, personal projects, or anything else. Attribution appreciated but not required.

---

## Quick Links

- [User Research & Problem Validation](discovery/user-research.md) — Validate the problem before you build
- [Data Strategy](discovery/data-strategy.md) — Plan your data pipeline
- [Model & Performance Requirements](strategy/model-requirements.md) — Define success metrics
- [Go-to-Market & Positioning](strategy/go-to-market.md) — Plan your market approach
- [PRD Framework](comms/prd.md) — Synthesize into a product plan

---

**Last updated:** 2026-05-03
```

- [ ] **Step 2: Verify file content**

```bash
wc -w README.md
# Should be ~600 words
```

- [ ] **Step 3: Commit**

```bash
git add README.md
git commit -m "feat: write root README with framework overview"
```

---

## Task 8: Final Polish & Git Push

**Files:**
- All `.md` files created above

- [ ] **Step 1: Review all files for consistency and quality**

```bash
find . -name "*.md" -type f | sort
```

Expected output:
```
./README.md
./comms/prd.md
./discovery/data-strategy.md
./discovery/user-research.md
./strategy/go-to-market.md
./strategy/model-requirements.md
```

- [ ] **Step 2: Verify no TODOs or placeholders**

```bash
grep -r "TODO\|TBD\|FIXME\|placeholder\|fill in\|add more" . --include="*.md"
```

Expected: No output (all files should be complete)

- [ ] **Step 3: Check all files are readable and well-formatted**

```bash
# Spot check one file to ensure formatting is correct
head -20 README.md
# Verify table renders properly, headers are clear, etc.
```

- [ ] **Step 4: Commit final version**

```bash
git add -A
git commit -m "feat: complete product framework with all templates and examples

- user research & problem validation framework
- data strategy framework  
- model & performance requirements framework
- go-to-market & positioning framework
- prd framework
- comprehensive root README with navigation

All frameworks include instructions, blank templates, and realistic detailed examples.
Ready for GitHub publication."
```

- [ ] **Step 5: Prepare for GitHub push**

Verify git status is clean:

```bash
git status
```

Expected: "On branch main" with "nothing to commit, working tree clean"

- [ ] **Step 6: Push to GitHub**

```bash
# First, verify your remote is set up
git remote -v

# If no remote, add it:
# git remote add origin https://github.com/YOUR_USERNAME/product-framework.git

# Push to main branch
git push origin main
```

Expected: Branch is updated, files are now live on GitHub

- [ ] **Step 7: Verify on GitHub web**

Open https://github.com/YOUR_USERNAME/product-framework in a browser.

Confirm:
- [ ] README.md renders properly
- [ ] All folders are visible (discovery, strategy, comms)
- [ ] All 5 framework files are present
- [ ] Markdown rendering looks correct (tables, headers, code blocks)
- [ ] Repository is public (check Settings → Visibility)

---

## Success Criteria

✅ All 5 frameworks complete with instructions, blank templates, and realistic examples
✅ Root README.md provides clear navigation and overview
✅ Folder structure reflects PM workflow stages (Discovery → Strategy → Comms)
✅ All files committed to git with clear commit messages
✅ Pushed to GitHub and publicly accessible
✅ No TODOs, placeholders, or incomplete sections
✅ Professional tone and polished presentation

---

## Notes

- Each framework file is self-contained; readers should understand the framework without needing to read others first
- Examples use realistic but hypothetical products to avoid any real company-specific information
- All content is written for a hiring manager / portfolio audience; tone is professional but accessible
- Markdown formatting is clean and uses consistent heading levels, emphasis, and structure
