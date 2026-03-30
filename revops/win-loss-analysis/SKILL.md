---
name: win-loss-analysis
version: 1.0.0
description: |
  AUTO-TRIGGER: Apply this skill when the user wants to run, structure,
  or improve a win/loss analysis program. Trigger phrases include:
  "win/loss analysis," "why are we losing deals," "why do we win,"
  "lost deal analysis," "closed lost reasons," "competitive losses,"
  "deal debrief," "why did we lose to [competitor]," "what does sales
  say about why we lose," "our closed lost data is useless," "I want
  to interview lost prospects," or any situation where the user is trying
  to understand the patterns behind deal outcomes.

  Also trigger when the user has win/loss data they need to synthesize,
  or when they want to turn win/loss findings into changes to ICP,
  messaging, pricing, or channel strategy.

  Do NOT trigger for general competitive intelligence, battlecard creation,
  or sales coaching. This skill is specifically about the structured
  diagnostic practice of analyzing deal outcomes and feeding the findings
  back into GTM decisions.
allowed-tools:
  - Read
  - Write
  - WebSearch
  - Edit
---

# Win/Loss Analysis: The Diagnostic That Improves Everything Downstream

This skill structures a win/loss analysis program that actually changes
how the team goes to market. Most companies do some version of win/loss
analysis. Almost none do it in a way that produces findings specific
enough to act on.

The failure mode is familiar: CRM closed/lost reason fields that contain
nothing useful ("not the right time," "went with competitor," "budget"),
post-loss debrief conversations with the sales rep that produce the rep's
perspective rather than the prospect's, and quarterly summaries that
confirm what leadership already believed rather than revealing something
that changes a decision.

This skill encodes the practices that produce findings specific enough
to change ICP definition, adjust messaging, inform pricing, and redirect
channel investment. The analysis is only useful if it feeds back into
something that changes.

---

## HOW TO SET UP THIS SKILL

Provide:

- What data you currently have on lost deals: CRM closed/lost reasons,
  rep debrief notes, anything else
- Whether you have access to lost prospects for direct interviews
- The time period you want to analyze
- The primary question you are trying to answer: is this about a specific
  competitor, a specific market segment, a pricing problem, or general
  pattern identification?
- What decisions you want to be able to make differently as a result

---

## Why CRM Closed/Lost Data Is Almost Always Wrong

Before building any analysis on CRM closed/lost data, understand its
limitations. CRM reasons are entered by sales reps under time pressure,
often days or weeks after the deal closed, based on whatever the rep
believes happened rather than what the prospect said. Four structural
problems make this data unreliable:

Reps rationalize losses. A deal lost because the rep did not follow up
fast enough, or because the demo was poorly matched to the use case,
will be logged as "not the right time" or "lost to competitor." The rep
is not lying. They genuinely believe their interpretation. But the root
cause is invisible in the data.

Categories are too broad to be useful. "Lost to competitor" tells you
nothing about why the prospect chose the competitor. "Price" tells you
nothing about whether the price was objectively too high, whether the
value was not communicated, or whether the discount was offered too
late. Every category in a standard CRM picklist is several real reasons
collapsed into one useless label.

Reps only know what the prospect told them. Prospects do not always give
honest feedback during a sales process. They tell reps what is
comfortable rather than what is true. "We decided to go in a different
direction" is easier to say than "your champion left the company and
we lost momentum" or "your competitor's CSM flew out to meet with us
and yours never called back."

Selection bias on who logs what. Reps who lose deals they expected to
win log detailed notes. Reps who lose deals they expected to lose often
log quickly and move on. The CRM overrepresents competitive losses on
deals where the rep felt invested and underrepresents losses on deals
where the rep was never confident.

None of this means CRM data is useless. It means it must be treated
as one signal among several, not as ground truth.

---

## The Three Data Sources That Produce Reliable Findings

Source 1: Direct prospect interviews (most valuable, hardest to get)

A 20-minute conversation with a decision-maker at a company that
evaluated your product and chose not to buy produces more insight than
100 closed/lost CRM records. Prospects are often willing to share their
real reasoning once the sales process is over and there is no commercial
pressure in the conversation.

Who conducts the interview matters. The prospect will be more honest
with a neutral party (a RevOps leader, a product marketer, or an outside
researcher) than with the sales rep who lost the deal.

The five questions that produce the most useful findings:

"Walk me through your evaluation process. What triggered the search,
who was involved, and how did you approach the decision?"

"What were the two or three things that mattered most to your team
when you were making this decision?"

"What was your impression of [your company] during the evaluation?
What stood out, positively or negatively?"

"What ultimately drove the final decision?"

"Is there anything we could have done differently that might have
changed the outcome?"

Do not defend the product. Do not correct misconceptions during the
interview. The goal is to understand what the prospect believed, not
to re-litigate the sale.

Source 2: Rep debrief structured correctly

A rep debrief is most useful when it separates the rep's interpretation
from what the prospect actually said. These questions produce evidence:

"What did the prospect say, specifically, when they told you they
were going with someone else?"

"At what point in the process did you first sense the deal was at
risk? What happened that week?"

"Who was the main decision-maker and who else was involved in the
final decision? Did you have access to all of them?"

"If you were going to run this deal again knowing what you know now,
what would you do differently?"

"What did the competitor do that we did not do?"

Source 3: Pattern analysis across CRM data with corrected categories

Once you have enough interview and debrief data to understand the
real reasons, go back and re-code the CRM records. Apply the real
categories you have discovered to the full dataset.

---

## What to Analyze and What to Look For

The competitive loss pattern: When you lose to a specific competitor
repeatedly, the question is not "why is their product better?" The
question is "at what point in the evaluation did the outcome tip, and
what caused it to tip?"

The internal political loss pattern: Many deals are not lost to
competitors. They are lost because the champion left, the budget was
reallocated, the project was deprioritized, or the buying committee
could not reach alignment.

The messaging gap pattern: When prospects consistently name a capability
as the reason they chose the competitor, and that capability exists in
your product but was not communicated effectively, you have a messaging
gap, not a product gap. The fix is different.

---

## Feeding Findings Back Into GTM Decisions

Findings that should change ICP: You are consistently losing in a
specific vertical, company size band, or organizational structure.

Findings that should change messaging: Prospects consistently
misunderstand a key capability, or consistently name a benefit you
provide but did not lead with.

Findings that should change the sales process: You are losing deals
at a consistent stage. Investigate what happens at that stage.

Findings that should change pricing or contract structure: You are
consistently losing deals where the prospect cited total cost of
ownership, implementation timeline, or contract flexibility.

Findings that should change channel investment: You are winning in
accounts sourced through a specific channel at a higher rate than
accounts sourced through others.

---

## Running Win/Loss on Wins Too

Win/loss programs that only analyze losses miss half the picture.
The most useful question from a win interview: "At what point did you
decide you were going to go with us, and what caused that?"

---

## Output Rules

- Be direct about the unreliability of CRM closed/lost data. Do not
  treat it as ground truth. Flag its limitations before building
  analysis on it.
- The findings-to-decisions map is required. Win/loss analysis
  without a mapped decision is a report, not a diagnostic.
- Distinguish product gaps from messaging gaps explicitly. The fix
  for each is different.
- If the user does not have access to lost prospects for interviews,
  say so directly and adjust the plan.
- No em dashes. Use commas or periods.
