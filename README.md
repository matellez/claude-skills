# Claude Skills for B2B Marketing and RevOps

Practitioner-built behavior systems for Claude. Built by a demand
generation and RevOps leader with 20 years in B2B SaaS.

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

The distinction matters. A generic resume skill tailors bullets and
checks ATS compatibility. The resume optimizer in this repo does that
too, but it also selects between two pre-built resume variants based on
role type, reorders proof points to match what the specific job cares
about most, distinguishes stated requirements from narrative filler in
a job posting, and flags gaps worth addressing before you apply. That
logic does not come from a framework. It comes from 20 years of
applying to and hiring for Director-level roles in B2B SaaS.

The same applies to the competitive intelligence skill. There are
public skills that scrape LinkedIn ads and summarize competitor
messaging. This one is built for a candidate walking into an interview,
not a marketing team running a competitive analysis. It pulls funding
context, ownership structure, tech stack signals, culture indicators,
and delivers talking points and questions designed to show you
understand the business, not just the product.

That is what practitioner judgment looks like when it is encoded into
a skill.

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

**job-posting-analyzer**
Breaks down a job posting into what is actually required versus what
is narrative filler. Identifies real gaps versus stated preferences,
and tells you directly whether to apply, apply with adjustments, or
pass.

Trigger: paste a job posting and ask "how well do I match" or "should
I apply."

### Research and intelligence

**competitive-intelligence**
Researches a company before an interview. Searches the web for recent
news, funding and ownership context, tech stack signals, and culture
indicators. Delivers a structured brief with talking points and smart
questions tailored to the specific role and your background in demand
gen and RevOps.

Distinguishing feature: built for interview prep, not competitive
analysis. The output is oriented toward a candidate who needs to walk
in knowing the company cold, not a marketer tracking a rival.

Trigger: mention a company name alongside an interview or job
application.

### Writing

**b2b-outreach-humanizer**
Removes AI writing patterns from B2B marketing and sales copy. Built
on a specific voice profile for a B2B practitioner: direct, revenue
minded, no editorial inflation, no filler openers or closers. Goes
beyond generic "make this less AI" passes by targeting 25 specific
language and style patterns that appear in LLM output.

Trigger: any written content you will publish or send.

**linkedin-post**
Writes LinkedIn posts for B2B marketers and RevOps practitioners.
Four content types: original takes, AI tools and productivity, article
commentary, and content series posts. Each type has its own structure,
word count, and ending strategy. No "agree or disagree" endings. No
hashtag dumps. Opinions required.

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

---

## About the author

Manuel Valles Tellez. Director-level demand generation and RevOps
leader, 20 years in B2B SaaS. HubSpot advanced. Salesforce. 28 AI
certifications across Anthropic, Google, Microsoft, and the American
Marketing Association.

These skills were built for real job search and marketing work, not
as a theoretical exercise.

linkedin.com/in/manuelvallestellez
