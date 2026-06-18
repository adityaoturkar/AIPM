# Product Teardowns

Deep-dive analyses of products using the [AIPM Product Framework](../README.md#the-five-frameworks). Each teardown examines product strategy, user experience, business model, and competitive positioning through a product manager's lens.

## 📋 Available Teardowns

| Product | Category | Framework Focus | Read Time |
|---------|----------|-----------------|-----------|
| [AppleCare](applecare-teardown.md) | Services / Subscription | Business model, retention loops, service quality | ~10 min |
| [Turo](turo-teardown.md) | Marketplace / Mobility | Two-sided marketplace trust, host/guest dynamics, competitive positioning | ~10 min |
| [Robinhood](robinhood-teardown.md) | Fintech / AI Banking | AI-powered financial OS thesis, trust dynamics post-2021, Gold subscription LTV | ~11 min |

## How to Read a Teardown

Each teardown follows a structured format:

1. **TL;DR** — Key insights and strategic opportunities
2. **Product Snapshot** — Quick reference table (pricing, footprint, competitors)
3. **Why This Product** — What makes it interesting to analyze
4. **Target Users & Segments** — Who it's built for and observed behavior
5. **First-Run Experience** — Initial onboarding and decision moments
6. **Core User Journey** — The main workflow where value is delivered
7. **Feature Audit** — What works, what doesn't, hidden gems
8. **Design & UX Analysis** — How product design choices support strategy
9. **Business Model & Monetization** — Economics, pricing, revenue levers
10. **Competitive Positioning** — How it compares to alternatives
11. **Growth Loops** — Retention mechanisms and expansion opportunities
12. **What I'd Change** — Product recommendations (quick wins, medium bets, big swings)
13. **Open Questions** — Data gaps and unknowns
14. **Lessons for Builders** — Principles applicable to your own products

## Contributing a Teardown

Want to analyze a product? Follow these steps:

### 1. Pick a Product
Choose a product you're genuinely curious about. Avoid:
- Products you haven't used or researched deeply
- Products so new there's minimal public information
- Products primarily different from existing teardowns (look for variety in category/business model)

### 2. Structure Your Analysis
Use the 14-section format above. Aim for:
- **Depth:** 1,500–2,500 words total (10–15 min read time)
- **Specificity:** Concrete details (actual pricing, observed user behavior) over generic analysis
- **Opinion:** Your point of view on what works/doesn't work (this is a portfolio piece, not a neutral summary)
- **PM Rigor:** Connect observations back to the Product Framework sections (User Research, Data Strategy, Model Requirements, Go-to-Market, PRD)

### 3. Write It
Create a new `.md` file in this folder: `<product-name>-teardown.md`

Example header:
```markdown
# 🔍 Product Teardown: [Product Name]

> [One-sentence hook on what's interesting about this product]

**Author:** [Your Name]
**Date:** YYYY-MM-DD
**Read time:** ~X min
**Tags:** `#category` `#aspect1` `#aspect2`

---
```

### 4. Submit
- Add a row to the **Available Teardowns** table above with link, category, framework focus, and read time
- Create a pull request with your teardown file and README.md update
- Or if you have direct access: commit to main directly

---

## Template Sections

Note: These templates are meant for new `.md` files in this folder (e.g., `product-name-teardown.md`), not for the main README.md.

Below is a minimal template you can adapt:

```markdown
# 🔍 Product Teardown: [Product Name]

> [Engaging hook]

**Author:** [Your Name]
**Date:** YYYY-MM-DD
**Read time:** ~X min
**Tags:** `#tag1` `#tag2`

---

## 📌 TL;DR

[2-3 sentences on key insight + biggest opportunity]

---

## 🎯 Product Snapshot

| Attribute | Value |
|-----------|-------|
| **Product** | [Name] |
| **Category** | [Category] |
| **Launched** | [Date] |
| **Business Model** | [Model] |
| **Pricing** | [Price/range] |
| **Competitors** | [List] |

---

## 1. Why I Picked This Product

[Why is it interesting? What PM challenges does it highlight?]

---

## 2. Who Is This For?

[User segments, what jobs to be done, willingness to pay]

---

## 3. First-Run Experience

[Onboarding, key decision moments, friction]

---

## 4. Core User Journey

[Main workflow where value is delivered]

---

## 5. Feature Audit

[What works, what breaks, hidden gems]

---

## 6. Design & UX Analysis

[How product design supports strategy]

---

## 7. Business Model & Monetization

[Economics, pricing levers, revenue strategy]

---

## 8. Competitive Positioning

[Comparison to alternatives, moat, risks]

---

## 9. Growth Loops

[Retention, expansion, referral mechanisms]

---

## 10. What I'd Change

### Quick wins (≤1 quarter)
[3-5 concrete improvements]

### Medium bets (1-4 quarters)
[3-5 strategic enhancements]

### Big swings (1+ year)
[2-3 transformative ideas]

---

## 11. Open Questions

[Data gaps, unknowns, analysis limitations]

---

## 12. Lessons for Builders

[3-5 principles applicable to other products]

---

## 📚 Sources

- [Link 1]
- [Link 2]

---

<sub>This teardown is independent analysis. [Product name] is a trademark of [Company]. Observations based on [publicly available information / personal use] as of [date].</sub>
```

---

## Why Teardowns Matter

Product teardowns serve three purposes in your PM portfolio:

1. **Demonstrate thinking** — Show how you analyze real products against the Product Framework
2. **Deep dive examples** — Illustrate framework principles with concrete details (competitors use for this, user research methods, monetization tradeoffs)
3. **Building intuition** — Pattern-matching across products strengthens your PM judgment

---

**Last updated:** 2026-05-12
