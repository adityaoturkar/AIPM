# Master README Hub Design

**Date:** 2026-05-07  
**Purpose:** Create an integrated master README that serves as a portfolio navigation hub across all branches while highlighting Product Framework content  
**Audience:** Job candidates, PMs exploring frameworks, GitHub visitors looking for PM templates  
**Deliverable:** Enhanced README.md on main branch  

---

## Project Overview

**Goal:** Transform the main README into an integrated hub that helps visitors discover both the Product Framework (main branch) and PM Prompts Library (claude/pm-prompt-library-setup-6YvGV branch), with clear CTAs guiding them to the right content.

**Success Criteria:**
- Visitors immediately understand what's available across branches
- Clear pathways for different visitor types (product builders, interviewees, template seekers)
- Product Framework content remains discoverable and well-organized
- Professional portfolio presentation
- Minimal clicks to reach target content

---

## Current State

**Main branch:** Product Framework (5 templates: User Research, Data Strategy, Model Requirements, Go-to-Market, PRD)
**Other branch:** PM Prompt Library (prompts, discovery templates, strategy guides)
**Problem:** Visitors on main branch can't see what's on other branch; single-branch focus

---

## Design Approach: Integrated Master Hub

The master README on main branch will serve dual purposes:
1. **Navigation hub** for all branches with descriptions and links
2. **Entry point** for Product Framework with use-case guidance

### Structure

#### 1. Header & Quick Navigation
Position at the very top for immediate impact.

```
# AIPM Portfolio

A collection of PM frameworks, templates, and prompts for building AI products.

**Quick start:**
- **Building AI products?** Explore the [Product Framework](#product-framework) (frameworks, examples, use cases)
- **Prepping PM interviews?** Check the [PM Prompts Library](#pm-prompts-library) on a separate branch
- **Want templates?** See [PM Prompts Library](#pm-prompts-library) for reusable prompt structures
```

**Rationale:** Visitors see options immediately. Three distinct paths for different needs.

---

#### 2. Portfolio Overview Table
Shows all branches with content summary and audience.

```
| Branch | Content | Best For |
|--------|---------|----------|
| **main** | 5 AI product frameworks + detailed examples | PMs building AI products, understanding product methodology, interview prep |
| **claude/pm-prompt-library-setup-6YvGV** | PM prompts, discovery templates, decision frameworks | Interview prep with structured prompts, accelerating PM workflows, template reuse |
```

**Rationale:** Clear, scannable overview. Helps visitors choose the right branch without deep exploration.

---

#### 3. Getting Started — Use Case Guides
Targeted pathways for different visitor types.

**"I'm building an AI product and want a structured framework"**
- Start with [User Research & Problem Validation](discovery/user-research.md) — validate the problem
- Move to [Data Strategy](discovery/data-strategy.md) — plan your data pipeline
- Then [Model & Performance Requirements](strategy/model-requirements.md) — define success metrics
- Then [Go-to-Market & Positioning](strategy/go-to-market.md) — plan market approach
- Finally [PRD Framework](comms/prd.md) — synthesize into a complete product plan

**"I'm interviewing for a PM role and want to discuss product thinking"**
- Review the [Product Framework examples](discovery/user-research.md) to see how frameworks apply to real products
- Check the [PM Prompts Library](../../tree/claude/pm-prompt-library-setup-6YvGV) for interview prompts and talking points
- Practice articulating: How would you approach this product? What data would you need?

**"I want reusable PM templates and prompts for my team"**
- Explore the [PM Prompts Library](../../tree/claude/pm-prompt-library-setup-6YvGV) branch for structured prompts
- Use Product Framework templates as starting points for your own frameworks

**Rationale:** Guides different visitor types directly to relevant content without forcing them to explore everything.

---

#### 4. Product Framework Section
Overview of the 5 frameworks with brief descriptions and links.

**The Five Frameworks**

| Framework | Stage | Purpose | Key Questions |
|-----------|-------|---------|----------------|
| [User Research & Problem Validation](discovery/user-research.md) | Discovery | Validate the problem is real before you build | Who has the problem? How bad is it? Are they willing to solve it? |
| [Data Strategy](discovery/data-strategy.md) | Discovery | Plan your data pipeline and address data challenges | What data do you need? Where will you get it? How will you ensure quality? |
| [Model & Performance Requirements](strategy/model-requirements.md) | Strategy | Define what "good enough" means for your model | What metrics matter? What performance targets will you hit? |
| [Go-to-Market & Positioning](strategy/go-to-market.md) | Strategy | Plan how you'll win in the market | Who should you target first? How are you different? How will you acquire customers? |
| [PRD Framework](comms/prd.md) | Comms | Communicate the complete product vision clearly | What are you building? How does it work? What's in/out of scope? |

**Why AI-Specific?**
- Data quality is a product input, not a side concern
- Model metrics don't directly translate to business outcomes
- AI products fail differently (ambiguity, bias, user expectations)
- Clear communication about capabilities AND limitations is critical

**Rationale:** Helps visitors understand framework structure and why these specific frameworks matter for AI products.

---

#### 5. Branch Navigation & How to Switch
Clear instructions for exploring the other branch.

```
## Explore the PM Prompts Library

The [PM Prompts Library](../../tree/claude/pm-prompt-library-setup-6YvGV) branch contains structured prompts and templates for:
- PM interviews (behavioral questions, case studies, frameworks)
- Discovery work (user research, competitive analysis)
- Strategy & planning (roadmapping, OKRs, positioning)

To explore it:
1. Click the branch dropdown at the top of this page
2. Select `claude/pm-prompt-library-setup-6YvGV`
3. Browse the content

Or: [Open PM Prompts Library directly](../../tree/claude/pm-prompt-library-setup-6YvGV)
```

**Rationale:** Makes it obvious how to navigate between branches without confusion.

---

#### 6. Footer
- Brief note on what this portfolio is (PM methodology + templates)
- License (freely shared)
- Last updated date
- GitHub stats (branches, commits)

---

## Content Organization

**Files affected:**
- README.md (main) — Enhanced with master hub structure

**Files unchanged:**
- discovery/user-research.md through comms/prd.md — Keep existing content
- Internal docs (specs, plans) — Stay in docs/superpowers/
- Other branches — Remain independent

---

## Success Metrics

✅ Visitors can see all branches without leaving main README
✅ Clear use-case pathways guide different visitor types
✅ Product Framework remains discoverable and well-organized
✅ Portfolio looks professional and intentional
✅ No more than 2-3 clicks to reach any target content

---

## Visual/Formatting Elements

- **Tables** for branch overview and framework comparison
- **Headers** with clear hierarchy (H1 for title, H2 for sections, H3 for subsections)
- **Blockquotes** for "Getting Started" use cases (easier scanning)
- **Links** to branches and individual frameworks (GitHub-native navigation)
- **Consistent formatting** with existing README style

---

## Notes

- Master README serves as both portfolio index AND framework entry point
- Avoids cognitive overload by providing multiple entry pathways
- Respects existing Product Framework structure (no reorganization needed)
- GitHub-native navigation (branch dropdown, links)
- Can be expanded later if more branches/projects are added
