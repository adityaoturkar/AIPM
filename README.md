# Product Framework

**Comprehensive PM methodology and template system for building AI products**

## What Is This?

This is a personal framework for product management in AI—not a generic playbook. It's built from real experience shipping AI products and solving the unique challenges they present: managing model uncertainty, defining metrics that matter, anticipating failure modes, and setting stakeholder expectations when outcomes are genuinely unpredictable.

This framework is designed for PMs, founders, and anyone building AI products who wants a structured approach to thinking through discovery, strategy, and communication. Whether you're working at a company or on your own project, these templates and frameworks help you ask the right questions before building.

## The Five Frameworks

| Framework | Stage | Purpose | Key Questions |
|-----------|-------|---------|----------------|
| **User Research & Problem Validation** | Discovery | Validate the problem and solution fit with data | What's the user pain? Can you measure it? Is it worth solving? |
| **Data Strategy** | Discovery | Define data requirements and collection strategy | What data do we need? How do we collect and maintain it? |
| **Model & Performance Requirements** | Strategy | Define success metrics that connect to business outcomes | What model performance matters? What are our acceptance criteria? |
| **Go-to-Market & Positioning** | Strategy | Understand competitive landscape and positioning | Who else is solving this? What's our unfair advantage? |
| **PRD Framework** | Comms | Craft the story and requirements of why this product exists and why now | What are the core requirements? Who should care and why? |

## How to Use This Repository

**For learning:** Each framework folder contains templates, checklists, and real examples. Read through to understand the PM approach.

**For your own projects:** Copy templates, adapt them to your product, and use them as you work. These are starting points, not final answers.

**For interviews:** Study the frameworks to discuss PM thinking in AI products. Reference them when talking through product decisions. This shows you have a systematic approach to messy problems.

## The Three Product Scenarios

This framework covers three core AI product types:

1. **Writing Assistant** — AI that augments human creativity (e.g., drafting, editing, ideation)
2. **Search** — AI that retrieves and synthesizes information (e.g., semantic search, multi-source Q&A)
3. **Recommendation System** — AI that predicts user preferences (e.g., personalization, ranking)

Each scenario has unique challenges: writing tools must preserve voice, search must handle ambiguity, recommendations must balance exploration and exploitation. The frameworks apply to all three, but the specific questions and metrics differ.

## What Makes These AI-Specific?

Traditional PM frameworks fall short for AI products. Here's why:

- **Data as a product input.** Your product's output quality depends directly on training data quality, labeling, and continuous improvement pipelines. This is new—it's part of your product strategy, not just engineering.

- **Model vs. business metrics.** A model can be technically accurate (95% F1 score) but commercially useless (users don't trust it). You need frameworks that connect model performance to business outcomes.

- **Failure mode thinking.** Shipping a SQL bug is different from shipping a model that hallucinates. AI products fail in silent, subtle ways. You must anticipate failure modes before they reach users.

- **Expectation setting.** Users don't understand AI limitations. Your job is to set realistic expectations about what the product can and can't do, and to communicate uncertainty clearly.

## How to Contribute

This is a personal framework, and it evolves. If you've used these templates and have feedback, suggestions, or real examples that improve them, pull requests are welcome.

## License

Freely shared. Use, adapt, and learn from this framework however you'd like.

## Quick Links

- [User Research & Problem Validation](discovery/user-research.md)
- [Data Strategy](discovery/data-strategy.md)
- [Model & Performance Requirements](strategy/model-requirements.md)
- [Go-to-Market & Positioning](strategy/go-to-market.md)
- [PRD Framework](comms/prd.md)

---

**Last updated:** May 3, 2026
