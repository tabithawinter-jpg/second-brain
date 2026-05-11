# CLAUDE.md

> This is the root operating manual for your second brain. Claude reads this file at the start of every session in this folder. It tells Claude who you are, what matters to you, and where to find more detail.
>
> The `{{placeholders}}` below are filled in automatically when you run the `/second-brain` skill. You can edit anything by hand afterwards, but the skill is the easier way: edit `second-brain-intake.md` and re-run.

---

## Who this brain belongs to

**{{name}}**, {{role_one_liner}}.

Working pattern: {{working_pattern}}.

---

## What the business does

{{business_one_liner}}

Full description: [[context/about-business.md|about-business]].

---

## What I sell

See [[context/services.md|services]] for the full list. The short version: {{services_short}}.

---

## Who I serve

See [[context/icp.md|icp]] for the full ideal-client picture. The short version: {{icp_short}}.

---

## What matters right now

The next 90 days, in order:

{{priorities_list}}

Full detail in [[context/priorities.md|priorities]].

---

## Voice and never-assume

- Voice register and writing samples: [[references/voice.md|voice]]. Match this.
- Things Claude must never assume or get wrong: [[context/never-assume.md|never-assume]]. Read this before drafting anything client-facing.

---

## Files in this brain

Populated context (read these to understand the business):

{{populated_context_files}}

Populated references:

{{populated_reference_files}}

---

## How to use this brain

- Ask questions in plain language. Claude will use the files above to ground its answers in your actual business.
- To update the brain, edit `second-brain-intake.md` and re-run `/second-brain`. Previous file versions back up to `archives/`.
- To add an AI employee, run `/hire`. The employee leans on this brain.

---

*This brain was built with the `/second-brain` skill from the [Build Your Second Brain with Claude](https://github.com/<owner>/second-brain) bootcamp kit.*
