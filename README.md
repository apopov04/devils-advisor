# Devil’s Advisor

A lightweight agent skill for blunt, creative advice on making a CV more convincing for a particular job.

Give your agent your CV and a posting. It identifies the weak spot, ranks changes, suggests relevant additions and asks a few useful follow-up questions. Suggestions are role-aware rather than a canned list of projects.

It distinguishes supported reframing, experience to surface or create, and—when explicitly requested—exaggerated or invented claims. Hypothetical material is labeled so the user can see what goes beyond their supplied history. It does not promise an ATS result or knowledge of private employer filters.

## Use it

1. Clone this repository, or choose **Code → Download ZIP** and extract it.
2. Install the folder following your agent’s skill instructions, or give it [SKILL.md](SKILL.md) directly.
3. Provide your CV and the full posting, then try:

> Use Devil’s Advisor to identify what my CV is missing for this role. Be blunt, suggest stronger positioning and a few relevant additions, and keep factual and hypothetical material clearly distinguished.

Optional [Ashby source notes](references/ashby-notes.md) explain the limits of vendor-specific claims. The internal skill identifier remains `unempluzzed-cv-check`, so existing invocations keep working.

## Privacy and cost

This repository contains instructions, not an upload service. Your agent and model provider process documents under their own settings. No separate API key or service is required; your agent’s usual usage costs may apply.

Created for [Unempluzzed](https://unempluzzed.com).
