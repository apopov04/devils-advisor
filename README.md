# Requirement Fulfiller

A lightweight agent skill for a blunt, job-specific CV teardown with concrete replacement lines.

Give your agent your CV and a job posting. It identifies the most consequential evidence problem first, then returns:

- Ranked fixes for missing requirements, buried evidence and weak claims.
- Common expectations, clearly marked as inferred.
- Standout evidence worth highlighting for this particular role.
- Before/after lines grounded in your experience, useful cuts, and focused questions that unlock stronger edits.
- Cheeky, role-specific project ideas when the CV is thin, followed by a concrete plan: what to build, what counts as finished, and what evidence to keep.

It does not submit applications, invent qualifications or claim to reproduce an employer’s private filters.

## Use it

1. Clone this repository, or choose **Code → Download ZIP** and extract it.
2. If your agent supports skill folders, install the folder following that agent’s instructions.
3. Otherwise, give the agent [SKILL.md](SKILL.md) directly and ask it to follow the instructions.
4. Provide your CV and the full job posting, then try:

> Use Requirement Fulfiller to compare my CV with this job posting. Be blunt about weak evidence. Prioritize the fixes that matter for this role, write replacement lines from my actual experience, and ask focused questions about missing details.

The main skill is self-contained. Optional [Ashby source notes](references/ashby-notes.md) explain the limits of vendor-specific claims. [Agent metadata](agents/openai.yaml) supplies a display name and example prompt for supporting agents.

## Privacy and cost

This repository contains instructions, not a CV upload service. Your agent and model provider process documents under their own settings. The skill needs no separate API key or paid service, but your agent’s normal usage costs may apply.

## Scope

This is a candidate editing aid. “Not demonstrated in the CV” does not mean a person lacks a skill. The skill separates confirmed facts from proposed additions and does not assign an Ashby score or predict hiring outcomes.

Created for [Unempluzzed](https://unempluzzed.com).
