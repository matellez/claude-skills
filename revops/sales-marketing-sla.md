---
name: sales-marketing-sla
version: 1.0.0
description: |
  AUTO-TRIGGER: Apply this skill when the user wants to build, fix, or
  document the agreement between sales and marketing around lead quality,
  lead handoff, and follow-up expectations. Trigger phrases include:
  "MQL definition," "sales-marketing SLA," "lead handoff," "sales isn't
  following up," "marketing leads are bad," "what counts as an MQL,"
  "sales and marketing alignment," "service level agreement," "lead
  routing," or any conversation where sales and marketing are in
  disagreement about lead quality or pipeline contribution.

  Also trigger when the user is setting up a new CRM or rebuilding the
  lead management process and needs to define how marketing hands leads
  to sales and what sales commits to doing with them.

  Do NOT trigger for general RevOps questions not related to the
  marketing-to-sales handoff, or for content strategy and copywriting
  requests. This skill is specifically about defining, documenting, and
  enforcing the agreement between marketing and sales around what a
  qualified lead is and what happens to it.
allowed-tools:
  - Read
  - Write
  - Edit
---

# Sales-Marketing SLA: Defining, Documenting, and Enforcing the Handoff

This skill builds the operational agreement between marketing and sales
around lead quality and follow-up. The marketing-to-sales handoff is
the most common source of revenue leakage in B2B SaaS. Marketing
generates leads that sales does not work. Sales blames marketing for
bad lead quality. Marketing blames sales for ignoring good leads. Both
sides have data that supports their position. Neither side has a shared
definition of what a good lead actually is.

The problem is almost never lead quality or sales effort in isolation.
It is the absence of a written, agreed-upon, and measured definition
of what marketing is responsible for delivering and what sales is
responsible for doing with it. This skill builds that definition.

---

## HOW TO SET UP THIS SKILL

This skill works out of the box. For more specific output, provide:

- Average deal size and sales cycle length
- Current MQL definition if one exists
- Current SLA if one exists, even informally
- How many MQLs marketing generates per month and what percentage
  sales works within the expected timeframe
- The primary source of conflict between sales and marketing right now
- Whether this is being built from scratch or rebuilt after a breakdown

---

## Why Most MQL Definitions Fail

Most MQL definitions fail for one of three reasons.

**Reason 1: The definition was built by marketing without sales input.**

Marketing defined an MQL based on what data they could track: a form
fill, a content download, a demo request. Sales was told about the
definition after it was built. Sales never agreed to it, never believed
in it, and never prioritized MQLs that came from that definition.

**Reason 2: The definition is based on activity, not fit.**

An MQL defined as "any contact who downloads a whitepaper" captures
students, competitors, and consultants doing research. It does not
filter for the companies that can actually buy. Activity-based MQL
definitions produce high volumes of low-quality leads and erode sales
confidence in the MQL program entirely.

**Reason 3: There is no enforcement mechanism.**

A written MQL definition that lives in a slide deck and is not
enforced by the CRM is not a definition. It is a suggestion. Without
automatic lifecycle stage transitions, lead routing workflows, and
SLA tracking in the CRM, the definition is aspirational rather than
operational.

---

## Building the MQL Definition

A good MQL definition has two components: firmographic fit and
behavioral signal. Both must be present. Either alone is insufficient.

---

### Component 1: Firmographic fit

This defines the type of company that can buy. It should map directly
to the ICP and should be specific enough to exclude companies that
will waste sales time.

**Questions to answer with sales input:**

What company size range has the highest close rate historically?
What verticals are in scope for this year's sales plan?
Are there geographies or company stages that are explicitly out of scope?
What job titles or seniority levels indicate a real buyer versus a researcher?

**The output is a set of hard filters:**

A contact is not an MQL unless the company meets: company size between
X and Y employees, industry in [specific verticals], geography in scope,
and the contact holds a title that indicates purchase authority or
meaningful influence on the buying decision.

These filters should be applied automatically in the CRM. If a form
submission comes in from a company with 10 employees and the target
is 50-500, it should not become an MQL. It should become a lead that
goes into a nurture sequence, not a sales queue.

---

### Component 2: Behavioral signal

This defines what the contact has done to indicate they are actively
evaluating a solution. Firmographic fit without behavioral signal means
a company that could buy but has not shown interest. Behavioral signal
without firmographic fit means interest from someone who cannot buy.

**Signal tiers by strength:**

High-intent signals (auto-qualify if fit criteria met):
Demo request or free trial signup. Pricing page visit combined with
two or more additional page views in the same session. Repeated
website visits from the same contact within a 14-day window. Direct
inbound contact via phone or chat requesting information.

Medium-intent signals (qualify if combined with additional engagement):
Content download combined with email open and click within 7 days.
Webinar attendance with post-webinar follow-up link click. Case study
or ROI calculator engagement.

Low-intent signals (nurture, do not route to sales):
Single content download with no follow-up engagement. Newsletter
subscription. Conference badge scan with no follow-up digital
engagement.

**The scoring model:**

Assign point values to each signal based on observed correlation with
pipeline creation. High-intent signals should be weighted heavily.
Low-intent signals should be weighted minimally or excluded from MQL
scoring entirely.

Set a threshold score. Contacts who exceed the threshold and meet the
firmographic fit criteria become MQLs and route to sales. Contacts
who meet firmographic fit but are below the threshold stay in nurture.
Contacts who exceed the threshold but do not meet firmographic fit
stay in nurture with a different track.

**An important caution on scoring models:**

Do not make the scoring model so complex that it cannot be explained
in two sentences. If a sales rep asks "why did I get this lead?" and
the answer requires a spreadsheet, the model is too complex. Sales
needs to trust the model, and trust requires transparency.

---

## Defining the Sales SLA

The SLA is what sales commits to doing with every MQL. Without a
defined SLA, marketing has no basis for accountability when leads
are not worked, and sales has no agreed-upon expectation to hold
themselves to.

**The four elements of a functional SLA:**

**Response time:** How many business hours from MQL routing to first
sales contact attempt? Industry standard for high-intent leads is
under 4 hours for demo requests, under 24 hours for other high-intent
signals. Set the commitment based on what sales can actually deliver,
not what the ideal would be. A SLA that is violated 80% of the time
is worse than no SLA, because it establishes that the agreement
does not matter.

**Contact attempts:** How many outreach attempts is sales required
to make before a lead is marked as "worked and unresponsive"? Minimum
recommendation is five attempts across at least two channels (phone
and email) over a seven to ten business day window. A lead marked
as "no response" after one call is not a worked lead.

**Disposition requirement:** After working a lead, what dispositions
are available? Common options: converted to opportunity, disqualified
with a specific reason (budget, timing, not a fit, wrong contact),
or unable to reach after required attempts. The "unable to reach"
disposition should trigger a marketing re-engagement sequence, not
a permanent archive.

**Feedback loop:** When sales disqualifies a lead, they must provide
a specific reason. "Not interested" is not a specific reason. "Company
is too small, under 50 employees" is a specific reason that marketing
can use to tighten the MQL definition. The feedback loop is how the
MQL definition improves over time.

---

## Getting Sales Buy-In on the Definition

This is where most SLA initiatives fail. Marketing builds the
definition, presents it to sales, and is surprised when sales does
not adopt it.

**The right process:**

Do not present a finished MQL definition to sales. Facilitate the
conversation that produces the definition together. Run a session
with the sales leader and two or three reps. Start with the question:
"Tell me about the last three marketing leads that converted to
pipeline. What was different about those leads compared to the ones
that went nowhere?"

The answers to that question, collected from sales, become the
foundation of the MQL definition. When sales helped build it, they
own it. When marketing built it and handed it to them, they tolerate
it at best.

**The minimum viable agreement:**

If the full MQL definition process is too slow or politically complex
to complete, start with the minimum viable agreement: a written list
of the three things that disqualify a lead from ever being routed to
sales. Get sales to agree to those three disqualifiers in writing.
That is the floor. Everything else is refinement.

---

## CRM Configuration for the SLA

The SLA is only operational when it is enforced by the CRM. Everything
else is a policy document that depends on individual compliance.

**Required CRM configuration:**

Automatic lifecycle stage transitions: When a contact meets both
firmographic fit and behavioral signal threshold, the lifecycle
stage should automatically update to MQL without manual intervention.
If a rep has to manually change a lifecycle stage for a lead to be
counted, the data will be incomplete.

Automatic lead routing: When a contact becomes an MQL, the CRM should
automatically assign it to the correct owner based on territory,
company size, or vertical. Do not rely on a daily manual review of
the MQL queue.

SLA timer: Track the time between MQL creation and first sales
activity. This can be done with a custom date field in HubSpot or
a workflow that stamps a "first activity date" and calculates the
gap. Without this measurement, you cannot report on SLA compliance.

Disposition tracking: Create a required field that sales must complete
before moving a lead out of the MQL stage. No lead should be able to
move to "disqualified" or "no response" without a reason selected.

**SLA reporting requirements:**

Build a weekly report that shows: MQL volume by source, MQL to SQL
conversion rate, median time to first sales contact, disposition
breakdown for disqualified MQLs, and the number of MQLs aged more
than 72 hours without a sales contact attempt.

This report should go to both the marketing leader and the sales
leader at the same time. It is a shared accountability document,
not a marketing report card.

---

## Deliver the SLA Design

Output in this format:

```
SALES-MARKETING SLA DESIGN
[Company or team name if provided]
Built: [today's date]

CURRENT STATE ASSESSMENT
[What the existing handoff process looks like based on what the user
described. Where the friction points are. Whether this is a definition
problem, an enforcement problem, or a trust problem.]

MQL DEFINITION

Firmographic fit criteria (required, applied automatically):
- Company size: [range]
- Industries in scope: [list]
- Geographies in scope: [list]
- Qualifying titles: [list]
- Disqualifiers (immediate exclusions): [list]

Behavioral signal scoring:
- High-intent signals [point value each]: [list]
- Medium-intent signals [point value each]: [list]
- Low-intent signals [do not score or minimal weight]: [list]
- MQL threshold score: [number]
- Score + fit = MQL: [confirm logic]

SALES SLA

Response time commitment: [hours for each signal tier]
Contact attempt requirement: [number, channels, timeframe]
Required dispositions: [list with definitions]
Feedback requirement: [what sales must provide when disqualifying]

CRM CONFIGURATION REQUIRED

1. [Specific workflow or field to configure]
2. [Specific workflow or field to configure]
3. [Specific workflow or field to configure]
[Continue as needed]

SLA REPORTING DASHBOARD

Weekly metrics: [specific metrics with data source]
Who receives it: [both marketing and sales leadership]
Review cadence: [recommended meeting cadence to review together]

GETTING SALES BUY-IN

Session structure: [how to run the definition session with sales]
Minimum viable agreement: [what to get signed off on if full process stalls]
Who needs to be in the room: [required attendees and why]

RISKS
[The two or three most likely reasons this SLA will be built but not
adopted. Based on what the user has described.]
```

---

## Output Rules

- Never produce a generic MQL definition. Every definition should be
  specific to the company's ICP, deal size, and sales motion as
  described by the user.
- If the user has not provided ICP information, ask for it before
  building the definition. A definition without ICP context is a
  template, not an SLA.
- Be direct about the political dimension. SLA failures are usually
  trust failures, not technical failures. Acknowledge that and address
  the process for getting genuine sales buy-in, not just sales
  compliance.
- Do not recommend a scoring model so complex that it cannot be
  explained in two sentences. Complexity destroys adoption.
- Address rep-level non-compliance separately from leadership agreement.
  A sales leader can agree to an SLA in a meeting and reps can
  still ignore it. The CRM enforcement configuration is what closes
  that gap. Make sure the output includes specific workflows that
  require rep action rather than allowing leads to age passively.
- No em dashes. Use commas or periods.
