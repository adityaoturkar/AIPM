# Product Teardowns Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Add a /teardowns folder with a README index, move the AppleCare teardown into it, and integrate it into the main README for portfolio discovery.

**Architecture:** Three-task implementation. First, create the /teardowns/README.md with index structure and contribution template. Second, copy the AppleCare teardown file into /teardowns/. Third, update the main README.md to include a "Teardowns & Case Studies" section that links to the teardowns folder, maintaining consistency with the existing framework navigation style.

**Tech Stack:** Markdown, GitHub-native navigation (relative links and anchor references)

---

## File Structure

**Created:**
- `teardowns/README.md` — Index of teardowns, how to read them, template for contributions

**Modified:**
- `README.md` — Add "Teardowns & Case Studies" section before footer

**Moved:**
- `teardowns/applecare-teardown.md` — Copied from /Users/adirash/Downloads/applecare-teardown.md (source file unchanged)

---

## Task 1: Create /teardowns/README.md

**Files:**
- Create: `teardowns/README.md`

- [ ] **Step 1: Create the teardowns directory**

```bash
mkdir -p teardowns
```

Expected: Directory created (will show in `git status`)

- [ ] **Step 2: Write /teardowns/README.md**

```markdown
# Product Teardowns

Deep-dive analyses of products using the [AIPM Product Framework](../README.md#the-five-frameworks). Each teardown examines product strategy, user experience, business model, and competitive positioning through a product manager's lens.

## 📋 Available Teardowns

| Product | Category | Framework Focus | Read Time |
|---------|----------|-----------------|-----------|
| [AppleCare](applecare-teardown.md) | Services / Subscription | Business model, retention loops, service quality | ~10 min |

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
- Commit and push to main

---

## Template Sections

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

**Last updated:** 2026-05-08
```

- [ ] **Step 3: Verify file was created**

```bash
ls -la teardowns/README.md
```

Expected: File exists with size >2KB

---

## Task 2: Copy AppleCare Teardown to /teardowns/

**Files:**
- Copy: `/Users/adirash/Downloads/applecare-teardown.md` → `teardowns/applecare-teardown.md`

- [ ] **Step 1: Copy the AppleCare teardown file**

```bash
cp /Users/adirash/Downloads/applecare-teardown.md teardowns/applecare-teardown.md
```

Expected: File copied successfully

- [ ] **Step 2: Verify the file**

```bash
head -20 teardowns/applecare-teardown.md
```

Expected: Shows header with "🔍 Product Teardown: AppleCare"

- [ ] **Step 3: Check file integrity**

```bash
wc -l teardowns/applecare-teardown.md
```

Expected: Shows line count (should be 260+ lines based on the original)

- [ ] **Step 4: Commit the teardowns folder**

```bash
git add teardowns/
git commit -m "feat: add product teardowns section with AppleCare analysis

- Create teardowns/README.md with index, guide, and contribution template
- Add AppleCare detailed teardown (services, subscription, business model)
- Include structured format for future teardown contributions

Teardowns demonstrate framework application to real products and build PM intuition."
```

Expected: Shows "2 files changed, X insertions"

---

## Task 3: Update Main README.md with Teardowns Section

**Files:**
- Modify: `README.md` — Add "Teardowns & Case Studies" section before footer

- [ ] **Step 1: Read the current README.md to find insertion point**

```bash
grep -n "## Latest Updates\|## License\|---" README.md | head -10
```

Expected: Shows line numbers. Insert the teardowns section before "## Latest Updates" or "## License"

- [ ] **Step 2: Identify exact location in README.md**

The teardowns section should go after the "How to Use These Frameworks" section and before "## What's in This Portfolio". Find the line number of "## What's in This Portfolio" — the teardowns section goes right before it.

- [ ] **Step 3: Prepare the new section**

This is the exact markdown to insert before "## What's in This Portfolio":

```markdown
---

## 📚 Teardowns & Case Studies

See real-world product analysis using the frameworks. Each teardown applies the 5 Product Frameworks to a specific product, showing how to evaluate strategy, user experience, business model, and competitive positioning.

**[View all teardowns →](teardowns/README.md)**

**Current teardowns:**
- **[AppleCare](teardowns/applecare-teardown.md)** — Services subscription analysis covering retention, multi-device strategy, and service quality challenges

---

```

- [ ] **Step 4: Edit README.md to add the teardowns section**

Using a text editor or the Edit tool, insert the section from Step 3 right before the line containing "## What's in This Portfolio".

The exact location should be: After the "How to Use These Frameworks" section (which ends with "Use as reference in product reviews and planning"), add a blank line, then the teardowns section.

- [ ] **Step 5: Verify the edit**

```bash
grep -A 5 "Teardowns & Case Studies" README.md
```

Expected: Shows the new section with the link to teardowns/README.md and AppleCare teardown link

- [ ] **Step 6: Check link syntax**

Verify the links are correct (should use relative paths):
- `[View all teardowns →](teardowns/README.md)` — Link to teardowns folder README
- `[AppleCare](teardowns/applecare-teardown.md)` — Direct link to the teardown file

```bash
grep -E "\[.*\]\(teardowns/" README.md
```

Expected: Shows both links

- [ ] **Step 7: Commit the README update**

```bash
git add README.md
git commit -m "feat: add Teardowns & Case Studies section to main README

- Add cross-reference section linking to product teardowns
- Include AppleCare as first teardown example
- Position before portfolio details section
- Link to teardowns/README.md for full index"
```

Expected: Shows "1 file changed, X insertions"

---

## Task 4: Final Verification

**Files:**
- Verify: `teardowns/README.md`
- Verify: `teardowns/applecare-teardown.md`
- Verify: `README.md`

- [ ] **Step 1: Verify folder structure**

```bash
find teardowns -type f -name "*.md" | sort
```

Expected: Shows:
```
teardowns/README.md
teardowns/applecare-teardown.md
```

- [ ] **Step 2: Verify teardowns/README.md contains required sections**

Check that `/teardowns/README.md` has these sections:
- "# Product Teardowns" heading
- "Available Teardowns" table with AppleCare entry
- "How to Read a Teardown" section
- "Contributing a Teardown" section
- Template sections
- "Why Teardowns Matter" section

```bash
grep -E "^# Product Teardowns|Available Teardowns|How to Read|Contributing|Why Teardowns" teardowns/README.md
```

Expected: Shows all 5 section headers

- [ ] **Step 3: Verify AppleCare teardown is in place**

```bash
head -1 teardowns/applecare-teardown.md && tail -1 teardowns/applecare-teardown.md
```

Expected: Shows header "# 🔍 Product Teardown: AppleCare" and footer with attribution

- [ ] **Step 4: Verify main README has teardowns section**

```bash
grep -A 3 "## 📚 Teardowns & Case Studies" README.md
```

Expected: Shows the teardowns section with links

- [ ] **Step 5: Verify link targets exist**

Check that both links in the new README section point to actual files:
- `teardowns/README.md` should exist and be readable
- `teardowns/applecare-teardown.md` should exist and be readable

```bash
test -f teardowns/README.md && echo "✅ teardowns/README.md exists" || echo "❌ teardowns/README.md missing"
test -f teardowns/applecare-teardown.md && echo "✅ teardowns/applecare-teardown.md exists" || echo "❌ teardowns/applecare-teardown.md missing"
```

Expected: Shows both ✅

- [ ] **Step 6: Check git status**

```bash
git status
```

Expected: No untracked files, no uncommitted changes. All changes should be committed.

- [ ] **Step 7: Verify recent commits**

```bash
git log --oneline -5
```

Expected: Shows the 2 new commits:
- "feat: add Teardowns & Case Studies section to main README"
- "feat: add product teardowns section with AppleCare analysis"

---

## Task 5: Push to GitHub

**Files:**
- Push: All committed changes to origin/main

- [ ] **Step 1: Push to GitHub**

```bash
git push origin main
```

Expected: Shows "X files changed, Y insertions" and confirms push to origin/main

- [ ] **Step 2: Verify on GitHub web**

Visit: https://github.com/adityaoturkar/AIPM

Check:
1. Main README displays "Teardowns & Case Studies" section
2. Links are blue and clickable
3. Click "View all teardowns →" link — should show teardowns/README.md with full index
4. Click AppleCare link — should show the teardown with proper formatting
5. Teardowns section is in the correct position (before "What's in This Portfolio")

- [ ] **Step 3: Verify teardowns folder structure on GitHub**

Navigate to `/teardowns` folder on GitHub. Verify:
- `README.md` is visible and opens with full content
- `applecare-teardown.md` is visible and opens with proper formatting
- Both files are readable on GitHub web

---

## Success Criteria

✅ /teardowns folder created with README.md and AppleCare teardown  
✅ teardowns/README.md contains index, how-to-read guide, contribution template  
✅ AppleCare teardown copied and accessible at teardowns/applecare-teardown.md  
✅ Main README.md updated with "Teardowns & Case Studies" section  
✅ Section links to teardowns/README.md (full index) and teardowns/applecare-teardown.md (direct link)  
✅ All changes committed with clear messages  
✅ Changes pushed to GitHub and rendering correctly  
✅ Teardowns section appears in right position in README hierarchy  

---

**Plan ready for execution.**
