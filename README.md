# AI tools built by a practitioner

Practitioner-built tools, skills, and resources for B2B marketing,
demand generation, and RevOps. Built by a Director-level demand gen
and RevOps leader with 20 years in B2B SaaS.

---

## What a skill is

A Claude skill is a markdown file that tells Claude how to behave in a
specific situation. It defines when to trigger, what to do, in what
order, and what the output should look like.

The difference between a skill and a prompt: a prompt tells Claude what
to do once. A skill tells Claude how to think about an entire category
of work, every time, automatically.

---

## What makes these different

There are hundreds of Claude skills on GitHub covering marketing,
demand gen, resume optimization, and competitive research. Most encode
generic frameworks. These encode practitioner judgment.

The distinction matters. A generic RevOps skill tells you what lead
lifecycle stages are. These skills tell you why your pipeline is
stalling, what your HubSpot instance is actually broken on, how to
negotiate your ZoomInfo renewal down 20%, and how to get a sales team
to actually adopt a new tool instead of working around it. That judgment
comes from doing the work across a dozen B2B SaaS companies, not from
reading about it.

---

## Skills in this repo

### Job search

**resume-optimizer**
Paste a job posting. Claude scores your fit, selects the right resume
version based on role type, tailors bullets to mirror the job's
language for ATS, reorders accomplishments based on what the role
actually prioritizes, and delivers a ready-to-submit resume. Includes
a "before you apply" checklist with role-specific action items.

Distinguishing feature: version selection logic. Most resume skills
treat your resume as a single document. This one selects between a
demand gen variant and a RevOps variant based on the job title and
description, then tailors from there.

Trigger: paste or share any job posting.

**competitive-intelligence**
Researches a company before an interview. Searches the web for recent
news, funding and ownership context, tech stack signals, and culture
indicators. Delivers a structured brief with talking points and smart
questions tailored to the specific role.

Distinguishing feature: built for interview prep, not competitive
analysis. The output is oriented toward a candidate who needs to walk
in knowing the company cold.

Trigger: mention a company name alongside an interview or job
application.

---

### RevOps and demand gen

**hubspot-audit**
Diagnoses an existing HubSpot instance across six domains: deal
pipeline and stage design, workflow health, lead lifecycle and
routing, data hygiene, reporting and attribution, and integrations.
Produces a prioritized remediation plan with critical, high priority,
and low priority items.

Distinguishing feature: every other HubSpot skill on GitHub automates
CRM actions via API. This one audits the structural health of the
instance the way an experienced admin would on day one of a new role.

Trigger: any mention of auditing, cleaning up, or inheriting a
HubSpot instance.

**pipeline-health-reviewer**
Diagnoses why a B2B sales pipeline is stalling. Identifies which of
four root causes is responsible: stage definition problems, ICP and
qualification gaps, follow-up sequence gaps, or structural sales cycle
length. Delivers a prioritized fix list and a 30-day leading indicator
to track.

Distinguishing feature: treats pipeline problems as systems problems,
not sales performance problems. Fixes the infrastructure before
blaming the reps.

Trigger: any request to review pipeline health, diagnose deal velocity,
or understand why deals are stalling.

**martech-contract-auditor**
Prepares you for a SaaS vendor renewal or renegotiation. Searches for
current pricing benchmarks, audits your leverage across six categories
(usage vs. spend, contract timing, competitive alternatives, multi-year
value, bundle gaps, and tenure), and delivers a negotiation brief with
specific ask language and a walk-away position.

Distinguishing feature: no other public skill addresses the specific
leverage dynamics of a MarTech renewal. This one encodes what actually
moves vendors in a renewal conversation.

Trigger: any mention of a vendor renewal, SaaS contract negotiation,
or right-sizing a MarTech stack.

**abm-campaign-builder**
Builds a structured ABM program from account selection through
sales-marketing coordination and measurement. Covers account list
criteria and tier structure, channel and content mix by tier,
coordination cadence, and a measurement framework built around
account penetration rather than lead volume.

Distinguishing feature: generic demand gen skills exist. ABM-specific
skills that address tier structure, sales-marketing coordination, and
the right metrics do not.

Trigger: any request to build or improve an account-based marketing
program or named account targeting strategy.

**free-trial-designer**
Designs or diagnoses a B2B SaaS free trial program across five
structural decisions: trial gate, trial length, feature access,
activation sequence, and conversion framework. Anchors the program
design to the value moment, the specific in-product action that most
strongly predicts conversion to paid.

Distinguishing feature: no public skill addresses the structural
design of a B2B trial program. Most onboarding skills assume the
trial already exists. This one designs it from scratch or fixes what
is broken.

Trigger: any request to build, fix, or evaluate a free trial program
or trial-to-paid conversion.

**gtm-ai-adoption-rollout**
Builds a 90-day adoption plan for rolling out AI tools and new
workflows to a sales or marketing team. Diagnoses which of five
common failure modes applies (wrong incentive structure, one-time
training event, too much change at once, unidentified resisters, or
no adoption owner), then delivers a phased rollout plan with
manager coaching guidance and behavioral success metrics.

Distinguishing feature: every GTM skill on GitHub teaches Claude how
to do marketing tasks. This one addresses the organizational problem
of getting a sales and marketing team to actually use new tools.
Built from the experience of achieving 100% GTM team adoption across
HubSpot, Salesloft, and ZoomInfo at a B2B SaaS company.

Trigger: any mention of rolling out AI tools, low tool adoption,
getting rep buy-in, or change management for a GTM team.

**partner-marketing-infrastructure**
Builds the operational infrastructure of a B2B partner program: tier
structure with movement criteria, CRM attribution configuration for
partner-sourced vs. partner-influenced deals, deal registration
workflow and conflict resolution rules, joint go-to-market playbook,
and a measurement framework that isolates partner-sourced revenue
from direct revenue.

Distinguishing feature: every other partner skill mentions co-marketing
in a single line. This one goes four levels deeper on the operational
and attribution infrastructure that determines whether a partner
program produces measurable pipeline or just activity.

Trigger: any mention of building a partner program, partner pipeline
attribution, reseller programs, or co-sell infrastructure.

---

### Writing

**b2b-outreach-humanizer**
Removes AI writing patterns from B2B marketing and sales copy. Built
on a specific voice profile for a B2B practitioner: direct, revenue
minded, no editorial inflation, no filler openers or closers. Targets
25 specific language and style patterns that appear in LLM output.

Trigger: any written content you will publish or send.

**linkedin-post**
Writes LinkedIn posts for B2B marketers and RevOps practitioners.
Four content types: original takes, AI tools and productivity, article
commentary, and content series posts. Each type has its own structure,
word count, and ending strategy. No "agree or disagree" endings.
Opinions required.

Trigger: any request for a LinkedIn post or update.

---

## How to use these skills

1. Open Claude.ai
2. Create a Project (Projects give Claude persistent instructions
   across conversations)
3. In Project Settings, paste the contents of any skill file into
   the Custom Instructions field
4. Start a conversation. The skill runs automatically based on what
   you say.

You can stack multiple skills in one Project. They are designed to
work together without conflicting.

---

## Personalizing these skills for your own use

Some skills reference specific resume content, career history, and
role targets. To use them for your own job search, replace those
sections with your own background. The trigger logic, scoring
frameworks, and output structure transfer directly.

The RevOps and demand gen skills work out of the box with no
personalization required. Just add them to a Project and describe
your situation.

---

## About the author

Manuel Valles Tellez. Director-level demand generation and RevOps
leader, 20 years in B2B SaaS. HubSpot advanced. Salesforce. 28 AI
certifications across Anthropic, Google, Microsoft, and the American
Marketing Association.

These skills were built for real job search and marketing work, not
as a theoretical exercise.

linkedin.com/in/manuelvallestellez
