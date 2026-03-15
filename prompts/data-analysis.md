# Data Analysis Prompts

Prompts for metrics interpretation, experiment design, and dashboard planning.

---

### 1. Metric Drop Diagnosis

**Use when:** A key metric has moved unexpectedly and you need to systematically diagnose the root cause before jumping to conclusions.
**Output type:** Structured diagnosis framework + prioritized list of hypotheses

---

One of our key metrics has changed unexpectedly. Help me diagnose the root cause.

Metric: [METRIC NAME, e.g., "7-day retention", "checkout conversion rate"]
Change observed: [e.g., "dropped 12% week-over-week", "spiked 30% over 3 days"]
Time period: [DATE RANGE]
Current value: [X%] vs. previous value: [Y%]

Additional context I have:
- Recent product changes or releases: [LIST OR "NONE"]
- Recent marketing or traffic changes: [LIST OR "NONE"]
- Segments or cohorts where the change is concentrated: [E.G., "MOBILE ONLY", "NEW USERS", OR "DON'T KNOW YET"]
- Any external factors (seasonality, competitors, outages): [LIST OR "UNKNOWN"]

Please:
1. Give me a structured diagnosis checklist — ordered from most to least likely root cause category (data/instrumentation issues → external factors → product changes → user behavior shifts)
2. For each category, list 2–3 specific hypotheses I should investigate and the SQL query logic or analysis I'd run to test it
3. Identify the single hypothesis I should investigate first and why
4. Flag any data I should pull immediately before the signal degrades (e.g., session logs, A/B test data)

---

### 2. A/B Test Design Reviewer

**Use when:** You are designing an A/B test and want to pressure-test the setup before launching.
**Output type:** Test design critique with specific recommendations

---

I'm designing an A/B test for the following:

What we're testing: [CHANGE OR FEATURE BEING TESTED]
Hypothesis: We believe that [CHANGE] will [IMPROVE METRIC] for [USER SEGMENT] because [REASON]
Primary metric: [METRIC]
Secondary / guardrail metrics: [LIST THEM]
Control group: [DESCRIPTION]
Treatment group(s): [DESCRIPTION]
Traffic allocation: [e.g., 50/50, 80/10/10]
Planned test duration: [X DAYS/WEEKS]
Minimum detectable effect (MDE): [% CHANGE WE CARE ABOUT]
Current baseline metric value: [CURRENT VALUE]
Weekly traffic to this surface: [APPROXIMATE NUMBER]

Please review my test design and:
1. Validate whether my sample size and duration are sufficient to detect my MDE at 80% power and 95% confidence — flag if I'm underpowered
2. Identify any threats to validity: novelty effects, network effects, seasonal confounds, or selection bias in my traffic split
3. Check my metric choices: is my primary metric the right one, and are my guardrail metrics comprehensive?
4. Flag any ethical or user experience risks in the experiment design
5. Suggest one change to improve the test's rigor or speed up time-to-decision

---

### 3. Dashboard & Metrics Framework Builder

**Use when:** You are defining the metrics and dashboard structure for a new product area or team.
**Output type:** Tiered metrics framework (North Star → L1 → L2) with dashboard layout recommendations

---

Help me design a metrics framework and dashboard for [PRODUCT AREA OR TEAM].

Product area: [DESCRIPTION]
Primary user action we care about: [e.g., "complete a booking", "publish a post", "invite a teammate"]
Business model: [e.g., subscription SaaS, marketplace, ad-supported]
Team mission: [ONE SENTENCE]
Current stage: [EARLY / GROWTH / MATURE]

Key stakeholders who will use this dashboard:
- [ROLE 1]: needs to understand [WHAT THEY CARE ABOUT]
- [ROLE 2]: needs to understand [WHAT THEY CARE ABOUT]

Please produce:
1. A North Star metric recommendation with a rationale — this should reflect user value AND business value
2. A tiered metrics tree:
   - L1 (3–4 metrics): Leading indicators that predict the North Star
   - L2 (2–3 metrics per L1): Diagnostic metrics that explain L1 movements
3. A list of 3–5 guardrail metrics we should always monitor to catch unintended consequences
4. A recommended dashboard layout with sections, chart types, and the primary audience for each section
5. One metric I should avoid tracking at the top level, and why (often a vanity metric)
