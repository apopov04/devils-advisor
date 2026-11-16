---
name: unempluzzed-cv-check
description: Compare a candidate's CV with a specific job posting to find missing requirements, terminology mismatches, relevant unstated expectations, and standout evidence worth adding. Suggest concise, evidence-backed changes; do not predict an ATS result. Use for job-specific CV gap checks rather than generic resume formatting or recruiter-side candidate ranking.
---

# Requirement Fulfiller

Help a job seeker answer: **What useful information is missing from my CV for this particular role?** Produce a short, prioritized set of additions and wording changes. This is a candidate's editing aid, not a hiring evaluation.

## Inputs and scope

Use the candidate's CV and the target job posting. Accept pasted text or readable files. If one is missing, ask for that input. If a posting link cannot be accessed, ask for pasted text rather than guessing its requirements. Review the extracted CV text for missing sections or scrambled reading order before drawing conclusions; distinguish extraction problems from absent evidence.

Use facts the candidate has provided in this conversation as well as the CV. Do not submit applications or contact employers as part of a CV check. Do not upload the CV to another service merely to run this skill. Use the agent's existing document-reading and reasoning capabilities; no extra API key, scraper, or scoring service is required. The agent's own provider and data settings still apply.

## Compare the role with the candidate's evidence

Separate the following, preserving the wording and priority of the posting:

- **Stated requirements:** explicitly required skills, experience, credentials, responsibilities and eligibility conditions. Keep preferred qualifications separate from must-haves. An "A or B" requirement does not require both.
- **Common expectations:** relevant fundamentals the posting leaves unstated. Mark these as inferred, explain the connection to this role, and avoid presenting a generic checklist as employer policy.
- **Standout opportunities:** specific evidence that would strengthen the application beyond the baseline. Tie each suggestion to the employer's stated work, stage, challenges or priorities. For example, a customer-facing React role may benefit from accessibility, performance or testing outcomes; an early product team may value ownership of a shipped feature. These are contextual recommendations, not facts about a hidden recruiter filter.

For each important requirement or opportunity, locate a supporting CV passage or candidate-provided fact. Quote the relevant line briefly. Report **not demonstrated in the supplied CV** rather than concluding the person lacks the skill. A skills-list mention establishes a mention, not project depth, years of experience, leadership or a business result.

### Terminology and precision

Recognize credible aliases and offer the posting's wording where it improves clarity. Preserve actual meaning and scope. Examples:

- "Built dashboards using React" → "Built dashboards using React.js" when the posting uses React.js.
- "Deployed services on AWS" → "Deployed services on Amazon Web Services (AWS)" when expanding the acronym is helpful.
- React Native is not sufficient evidence of React web application work.
- Java and JavaScript are different technologies; general cloud experience does not establish AWS experience.
- Academic, personal and professional experience remain labeled accurately; do not silently turn a project into employment.

Do not add a missing skill, qualification, employer, responsibility, date, duration, achievement or metric as an established fact unless supported. When a recommendation requires new information, ask a focused question and give a clearly conditional example. Use placeholders for unknown outcomes, not invented percentages. A date range covering overlapping roles does not establish additive years of experience.

## Return a lightweight action list

Start with the two or three highest-value changes. Usually five to eight recommendations are enough; use fewer when the evidence is sparse. Keep three visibly distinct groups when they contain useful items:

1. **Missing requirements and wording fixes**
2. **Common expectations to confirm**
3. **What could make this application stronger**

For each item, include only what helps the candidate act:

- The requirement, or the posting signal behind an inferred suggestion.
- What the CV currently demonstrates, with a short evidence quote when available.
- Why adding or clarifying it matters for this role.
- Where to put it and suggested wording, marked **ready to use** if fully supported or **use only if true** if confirmation is needed.

Do not force a numerical match score, hiring probability, universal "ATS score" or promised pass rate. A useful answer may say the CV already covers the role well. Do not label every absent nice-to-have a critical gap.

End with a small set of questions that would unlock the strongest edits, rather than interrupting analysis with one question per missing term. If the user has not done something, suggest a realistic project or learning step separately from changes they can make to the CV today.

Only rewrite the whole CV or edit its file when the user asks. Otherwise return recommendations and proposed lines, preserving the original document. When editing is requested, show a concise change summary and keep unconfirmed additions out of the final CV.

## Ashby and other application systems

Using Ashby does not tell us which features an employer enabled, which internal criteria they set or which search a recruiter runs. Optimize clarity and coverage against the public posting and the candidate's evidence. Label any inferred evaluation criteria as our interpretation.

If asked specifically about Ashby filtering, consult [the source notes](references/ashby-notes.md) when available. Public documentation describes several search modes and configurable AI review; it does not establish a universal React/React.js failure. If this file was provided by itself, explain those limits without requiring the reference file. This skill also works for postings on other systems.
