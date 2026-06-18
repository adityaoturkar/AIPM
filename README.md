# AIPM Portfolio

A collection of AI product management frameworks, templates, and prompts for building AI products.

## Quick Start

Pick what you're looking for:

- **Building an AI product?** Explore the [Product Framework](#the-five-frameworks) — validated PM methodology for AI products with detailed examples
- **Prepping for PM interviews?** Check the [PM Prompts Library](#explore-the-pm-prompts-library) for structured interview prep and decision frameworks
- **Want reusable templates?** See [PM Prompts Library](#explore-the-pm-prompts-library) for prompt structures and accelerators

---

## What's Available

| Branch | Content | Best For |
|--------|---------|----------|
| **main** (you are here) | 5 AI product frameworks + detailed realistic examples | Building AI products, understanding PM methodology, interview prep |
| **[claude/pm-prompt-library-setup-6YvGV](../../tree/claude/pm-prompt-library-setup-6YvGV)** | PM prompts, discovery templates, strategy guides, decision frameworks | Interview prep with structured prompts, accelerating PM workflows, reusable templates |

---

## Getting Started

### "I'm building an AI product and want a structured framework"

Follow this sequence:

1. **[User Research & Problem Validation](discovery/user-research.md)** — Validate the problem is real
   - Understand users, their pain points, willingness to pay
   - Example: AI Writing Assistant market validation with interview data
   
2. **[Data Strategy](discovery/data-strategy.md)** — Plan your data pipeline
   - Define what data you need, where to get it, how to ensure quality
   - Example: AI Search Product with data sourcing, labeling, compliance costs
   
3. **[Model & Performance Requirements](strategy/model-requirements.md)** — Define what "good enough" means
   - Success metrics, business impact, fairness constraints
   - Example: AI Recommendation System with CTR targets, disparity thresholds, rollout gates
   
4. **[Go-to-Market & Positioning](strategy/go-to-market.md)** — Plan how you'll win
   - Target customer, value prop, competitive positioning, CAC:LTV
   - Example: AI Writing Assistant with 3-phase GTM and unit economics
   
5. **[PRD Framework](comms/prd.md)** — Synthesize into a product plan
   - Requirements, workflows, technical approach, risks, timeline
   - Example: AI Search Product with edge cases, architecture, risk mitigations

### "I'm interviewing for a PM role and want to discuss product thinking"

- **Review the frameworks** — See how real PM thinking applies to AI products
  - Read [User Research](discovery/user-research.md) to understand problem validation
  - Skim [Model Requirements](strategy/model-requirements.md) to understand metric thinking
  - Study [Go-to-Market](strategy/go-to-market.md) to see unit economics reasoning

- **Explore PM Prompts Library** — [Switch to the pm-prompt-library branch](../../tree/claude/pm-prompt-library-setup-6YvGV) for structured interview prep
  - Discovery prompts for your own product thinking
  - Strategy frameworks for discussing roadmaps
  - Decision guides for case study discussions

- **Practice articulating** — Use frameworks to structure your thinking
  - How would you approach this product? (User Research)
  - What data would you need? (Data Strategy)
  - How would you measure success? (Model Requirements)
  - Who would you target first? (Go-to-Market)

### "I want reusable PM templates and prompts for my team"

- **PM Prompts Library** — [Switch to this branch](../../tree/claude/pm-prompt-library-setup-6YvGV) for:
  - Structured prompts for discovery, strategy, decision-making
  - Templates you can adapt for your team
  - Acceleration frameworks for common PM workflows

- **Product Framework** — Use frameworks here as templates:
  - Copy the blank template section from any framework
  - Fill in your own examples
  - Adapt to your context

---

## The Five Frameworks

These frameworks are specifically designed for AI product challenges: data quality as a product input, connecting model metrics to business outcomes, understanding failure modes differently, and setting clear expectations about AI capabilities.

| Framework | Stage | Purpose | Quick Start |
|-----------|-------|---------|------------|
| **[User Research & Problem Validation](discovery/user-research.md)** | Discovery | Validate the problem is real before you build | Who has the problem? How bad is it? Are they willing to solve it? |
| **[Data Strategy](discovery/data-strategy.md)** | Discovery | Plan your data pipeline and address data challenges | What data do you need? Where will you get it? How will you ensure quality? |
| **[Model & Performance Requirements](strategy/model-requirements.md)** | Strategy | Define what "good enough" means for your model | What metrics matter? What performance targets will you hit? |
| **[Go-to-Market & Positioning](strategy/go-to-market.md)** | Strategy | Plan how you'll win in the market | Who should you target first? How are you different? How will you acquire customers? |
| **[PRD Framework](comms/prd.md)** | Comms | Communicate the complete product vision clearly | What are you building? How does it work? What's in/out of scope? |

### Why AI-Specific?

These frameworks address challenges unique to AI products:

- **Data as a product input** — Unlike traditional software, AI quality depends directly on data quality. Every framework addresses data implications.
- **Model metrics ≠ business metrics** — The gap between "good accuracy on a benchmark" and "users actually find this useful" is large. These frameworks help you bridge it.
- **Different failure modes** — AI systems fail differently than traditional software (ambiguity, bias, user expectations). Frameworks include planning for these.
- **Expectation setting** — AI products need clarity about what they can and can't do. Frameworks help communicate limitations without losing trust.

---

## Explore the PM Prompts Library

The [PM Prompts Library](../../tree/claude/pm-prompt-library-setup-6YvGV) branch contains structured prompts and templates for:

- **PM interviews** — Behavioral questions, case studies, framework prompts, thinking guides
- **Discovery work** — User research prompts, competitive analysis templates, problem validation guides
- **Strategy & planning** — Roadmapping prompts, OKR frameworks, positioning templates, GTM decision guides

### How to Switch Branches

**Option 1: Use GitHub's branch dropdown**
1. Click the branch dropdown at the top of this page (currently showing "main")
2. Type or select `claude/pm-prompt-library-setup-6YvGV`
3. Explore the content

**Option 2: Direct link**
Open [PM Prompts Library](../../tree/claude/pm-prompt-library-setup-6YvGV) directly

---

## How to Use These Frameworks

**For your own product:**
1. Copy the "Key Sections" blank template from any framework
2. Fill in your own answers to the questions
3. Use the example as inspiration (but don't copy it — your context is different)

**For interviews:**
1. Read the framework overview to understand the thinking
2. Study the detailed example to see how PM reasoning works
3. Practice applying the framework to products you know
4. Reference the frameworks when discussing product strategy

**For your team:**
1. Treat the frameworks as starting templates
2. Adapt them to your context and product type
3. Share examples internally to align on PM thinking
4. Use as reference in product reviews and planning

---

## 📚 Teardowns & Case Studies

See real-world product analysis using the frameworks. Each teardown applies the 5 Product Frameworks to a specific product, showing how to evaluate strategy, user experience, business model, and competitive positioning.

**[View all teardowns →](teardowns/README.md)**

---

## What's in This Portfolio

This is a personal PM framework and template collection, publicly shared because it might be useful to you.

- **Not a commercial product** — These are tools I use and thinking I've developed
- **Freely shared** — Use for learning, interviews, personal projects, team adoption, or whatever serves you
- **Still evolving** — These frameworks improve as I work on more products and learn from feedback
- **GitHub-native** — Organized for easy browsing and reference

---

## Contributing

This is a personal framework reflecting my PM approach. If you find issues, suggestions, or want to adapt this for your context, that's great.

- **Issues/PRs** — Welcome for bugs, unclear sections, or broken links
- **Adaptations** — Fork and make it your own for your team or context
- **Feedback** — No formal process, but thoughtful input is always appreciated

---

## License

These templates and frameworks are shared freely. Use them for:
- Learning and understanding PM methodology
- Interview preparation
- Building your own frameworks
- Team training and acceleration
- Personal projects

No attribution required, though appreciated.

---

## Latest Updates

- **2026-05-07** — Added master hub with branch navigation and getting started guides
- **2026-05-03** — Completed all 5 frameworks with realistic detailed examples

---

**Last updated:** 2026-05-07
