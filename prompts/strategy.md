# Strategy Prompts

Prompts for roadmapping, prioritization, and product positioning.

---

### 1. Feature Prioritization with RICE

**Use when:** You have a backlog of features or bets and need a structured way to prioritize them for the next planning cycle.
**Output type:** RICE-scored prioritization table with reasoning

---

I need to prioritize the following features/initiatives for [PRODUCT NAME] going into [TIME PERIOD]:

[LIST YOUR FEATURES/INITIATIVES HERE — ONE PER LINE]

For each item, help me apply the RICE framework (Reach, Impact, Confidence, Effort) by:
1. Asking me up to 3 clarifying questions per item to estimate each RICE component — or if I've provided enough context, make reasonable assumptions and flag them
2. Producing a scored table with a RICE score for each item
3. Highlighting the top 3 by score and noting any that score similarly and might warrant a deeper discussion
4. Flagging any items that have high strategic value but low RICE scores — these may be worth a separate conversation

Business goal for this period: [PRIMARY METRIC OR OKR]
Team capacity: [NUMBER OF ENGINEERS / SPRINTS AVAILABLE]

---

### 2. Roadmap Narrative Builder

**Use when:** You have a prioritized list of initiatives and need to turn it into a coherent roadmap story for stakeholders.
**Output type:** Executive roadmap narrative (Now / Next / Later) with a strategic rationale

---

Here is our prioritized list of initiatives for the next [TIME HORIZON]:

Now (0–3 months): [LIST INITIATIVES]
Next (3–6 months): [LIST INITIATIVES]
Later (6–12 months): [LIST INITIATIVES]

Our company's strategic priorities are: [LIST 2–3 STRATEGIC PRIORITIES]
Our product's north star metric is: [METRIC]

Write a roadmap narrative that:
1. Opens with a 2–3 sentence framing of the product's current moment and strategic focus
2. Explains the "Now" priorities and why they come first (link to immediate business needs or technical dependencies)
3. Explains the "Next" priorities and what will need to be true to activate them
4. Describes the "Later" horizon as a directional vision, not a commitment
5. Closes with a sentence on what we are explicitly NOT doing and why

Tone: [EXECUTIVE BRIEF / ENGINEERING ALL-HANDS / INVESTOR UPDATE]

---

### 3. Competitive Positioning Analysis

**Use when:** You are defining or refining your product's positioning relative to competitors and need a structured framework.
**Output type:** Positioning analysis with differentiation recommendations

---

Help me analyze the competitive landscape for [PRODUCT NAME] in the [MARKET/CATEGORY] space.

Our product: [BRIEF DESCRIPTION OF WHAT YOU DO AND WHO YOU SERVE]

Key competitors:
- [COMPETITOR 1]: [BRIEF DESCRIPTION]
- [COMPETITOR 2]: [BRIEF DESCRIPTION]
- [COMPETITOR 3]: [BRIEF DESCRIPTION]

Our top 3 features/capabilities: [LIST THEM]
Our target customer: [ICP DESCRIPTION]

Please produce:
1. A positioning map narrative that describes where each competitor sits on the axes of [AXIS 1, e.g., "ease of use"] vs. [AXIS 2, e.g., "enterprise readiness"]
2. An analysis of the white space — underserved segments or unmet needs no competitor is addressing well
3. A recommended positioning statement using the format: "For [TARGET CUSTOMER] who [NEED], [PRODUCT] is the [CATEGORY] that [KEY BENEFIT], unlike [ALTERNATIVE] which [LIMITATION]."
4. The 2–3 biggest risks to this positioning over the next 12 months
