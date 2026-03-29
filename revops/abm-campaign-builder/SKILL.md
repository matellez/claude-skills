---
name: abm-campaign-builder
version: 1.0.0
description: |
  AUTO-TRIGGER: Apply this skill when the user wants to build, plan,
  or improve an account-based marketing program. Trigger phrases include:
  "ABM campaign," "named account targeting," "target account list,"
  "account-based," "we want to go after specific accounts," "enterprise
  accounts," "1:1 or 1:few marketing," or any request to build a
  coordinated sales and marketing program around a defined account list
  rather than broad demand generation.

  Also trigger when the user asks how to align sales and marketing around
  specific accounts or how to measure account penetration rather than
  lead volume.

  Do NOT trigger for general demand gen, inbound, or broad campaign
  planning that is not account-specific.
allowed-tools:
  - Read
  - Write
  - Edit
---

# ABM Campaign Builder: Account-Based Marketing Program Design

This skill builds a structured ABM program from account selection
through to sales-marketing coordination and measurement. It treats
ABM as a systems problem: the account list, the tier structure, the
channel mix, and the sales handoff all have to work together or the
program produces activity without pipeline.

---

## HOW TO SET UP THIS SKILL

Ask the user for the following context before proceeding:

- What product or service are they selling and to whom
- Average deal size and target company size range
- Whether they have an existing account list or are building one
- How many accounts they are targeting (rough number)
- What sales and marketing resources are available to run the program
- Whether they have intent data, a CRM, or marketing automation

If they have an existing program, ask what is and is not working
before redesigning it.

---

## The ABM Program Framework

A functional ABM program has five components. Build all five or
the program will not hold together.

---

### Component 1: Account selection and list building

This is where most ABM programs fail. The account list is built
from gut feel or a spreadsheet of logos someone wants to land, rather
than from data about which accounts are most likely to buy.

**How to build the right list:**

Start with closed-won data. Look at the last 12-24 months of deals
that closed and identify the patterns: company size, industry vertical,
tech stack, growth stage, geography, and buyer persona. That is your
ICP. Accounts that match that pattern are the highest-probability
targets.

Layer in intent data if available. Accounts that match the ICP and
are showing buying signals (researching relevant topics, visiting
competitor sites, hiring for roles that indicate a relevant initiative)
are the highest-priority targets.

Filter by sales capacity. An ABM list is only as good as the coverage
behind it. If sales can genuinely work 50 accounts at a time, the
list should be 50 accounts, not 500.

---

### Component 2: Tier structure

Not all ABM accounts get the same treatment. Tier structure defines
how resources are allocated across the list.

Tier 1 (1:1 programs, 5-20 accounts): Highest priority accounts.
Fully custom: personalized content, executive outreach, dedicated
sales attention. Marketing is essentially an extension of the account
team for these accounts.

Tier 2 (1:few programs, 20-100 accounts): High priority accounts
grouped by vertical, use case, or persona. Campaigns are personalized
to the cluster, not to the individual account.

Tier 3 (1:many programs, 100+ accounts): Scaled ABM. Accounts that
match the ICP but do not yet have enough signal to warrant Tier 1 or
2 investment. Programmatic targeting and intent-triggered outreach.

---

### Component 3: Channel and content mix

Tier 1: Direct mail, executive events, personalized video outreach,
custom content specific to their situation, LinkedIn direct messaging
coordinated with sales.

Tier 2: LinkedIn targeting by account list, personalized email
sequences, webinars by vertical, paid retargeting against account
lists, SDR outreach with account-specific context.

Tier 3: Programmatic display targeting by account list, LinkedIn
sponsored content, intent-triggered email sequences.

Content principle: Every content asset should speak to a specific
problem, not a generic benefit. The best ABM content makes the
account feel like it was written for them specifically.

---

### Component 4: Sales and marketing coordination

ABM only works when sales and marketing are operating from the same
account plan. For each Tier 1 account, maintain:

- Account overview: size, revenue, known tech stack, key initiatives
- Buying committee map: stakeholders, champion, blocker
- Current relationship status: cold, warm, active conversation
- Marketing plays in progress: what campaigns are running
- Sales plays in progress: active outreach, open opportunities
- Agreed next milestone: what both teams are working toward this quarter

Coordination cadence: Weekly or biweekly for Tier 1. Monthly for
Tier 2. Quarterly for Tier 3.

---

### Component 5: Measurement framework

ABM should not be measured by lead volume. It should be measured
by account penetration and pipeline influence.

Metrics that matter:
- Account coverage: what percentage of target accounts have at least
  one known contact engaged in the last 90 days
- Account penetration: what percentage have an open opportunity
- Pipeline from target accounts: dollar value of pipeline created
  from the target account list this quarter
- Win rate on target accounts vs. non-target accounts
- Cycle length on target accounts

What not to measure: MQL volume from ABM campaigns. ABM does not
produce MQLs. It produces account engagement. Measuring it like
inbound will make the program look underperforming when it is working.

---

## Deliver the ABM Program Plan

Output in this format:

```
ABM PROGRAM PLAN
[Company or team name if provided]
Built: [today's date]

PROGRAM OVERVIEW
[2-3 sentences on scope: accounts, tiers, primary 90-day objective]

ACCOUNT LIST CRITERIA
ICP definition: [firmographic and technographic criteria]
Tier 1 accounts: [number and selection criteria]
Tier 2 accounts: [number and selection criteria]
Tier 3 accounts: [number and selection criteria]
Data sources needed: [intent data, CRM, LinkedIn, etc.]

CHANNEL MIX BY TIER
Tier 1: [specific channels]
Tier 2: [specific channels]
Tier 3: [specific channels]

CONTENT REQUIREMENTS
[What content needs to be created or repurposed. Specific format
and audience, not generic.]

SALES-MARKETING COORDINATION PLAN
Review cadence: [how often and what format]
Account ownership: [who owns which tier]
Handoff definition: [when does marketing hand to sales]

90-DAY MEASUREMENT PLAN
Week 1-4: [what to track and what baseline to establish]
Week 5-8: [what signals indicate the program is working]
Week 9-12: [what to report and what decisions to make]

SUCCESS METRICS
Primary: [the one number that tells you the program is working]
Secondary: [supporting metrics]
What not to track: [metrics that will mislead you]

RISKS AND WHAT TO WATCH
[Two or three most likely failure points and how to address proactively]
```

---

## Output Rules

- Base the plan on what the user actually has available: list size,
  budget, headcount, and tool access.
- Be direct about whether they have enough resources for ABM at the
  scale they are describing. A 500-account Tier 1 program is not ABM.
- Name specific tools only if the user has mentioned them.
- No em dashes. Use commas or periods.
