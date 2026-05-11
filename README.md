# Second Brain Starter Kit

A starter second brain for creative founders, built with Claude.

Two skills, one repo:

- **`/second-brain`**: answer 8 questions, walk away with a working starter brain (folders, files, context).
- **`/hire`**: answer 6 more questions, walk away with a job description for your first AI employee. Drop the file straight into a Claude project as instructions.

Both skills run conversationally. The brain comes first; the employee leans on the brain.

This kit is part of the **Build Your Second Brain with Claude** bootcamp. The bootcamp teaches the architecture; this kit demonstrates the bare minimum that makes the architecture work.

---

## Two ways to use it

Pick the path that matches your comfort level. **Path B is the simpler default.** Path A is the upgrade once you're comfortable in Claude Code.

### Path B: Claude Cowork (recommended)

You don't need to know how `git` works. You don't need to install anything beyond Claude Desktop.

1. On this GitHub page, click the green **`<> Code`** button → **Download ZIP**.
2. Unzip on your computer. You'll get a folder called `second-brain-main`. Rename it to something you'll recognise (e.g. `my-brain`) and move it somewhere you can find again (e.g. `~/Documents/my-brain`).
3. Open **Claude Desktop**. In the left sidebar, click **Projects**, then click **+ New project** in the top right.
4. From the three options that appear, pick the third one: **Use an existing folder**.
5. A folder picker opens. Navigate to your `my-brain` folder and select it. The project name auto-fills as `my-brain`. Leave Instructions empty. Click **Create**.
6. The project opens with your folder already linked under "On your computer" in the right sidebar. In the chat box, ask: *"Please read `.claude/skills/second-brain/SKILL.md` and follow those instructions to build my second brain."*
7. Answer the 8 questions one at a time. Take your time. When the skill finishes, your brain is built.
8. To hire your first AI employee, in the same project: *"Please read `.claude/skills/hire/SKILL.md` and follow those instructions to hire my first AI employee."*

> *Why the long prompt instead of `/second-brain` or `/hire`?* Cowork doesn't yet auto-discover skill files the way Claude Code does. The natural-language prompt does the same job: it tells Claude to open the skill file and run it. Same outcome.

### Path A: Claude Code (faster once you're set up)

If you have Claude Code installed and you're comfortable running terminal commands:

```bash
git clone https://github.com/tabithawinter-jpg/second-brain.git my-brain
cd my-brain
claude
```

Then in Claude Code: type `/second-brain`, answer the 8 questions, then `/hire` for the 6 employee questions.

---

## What you'll get

After running `/second-brain` you'll have:

```
my-brain/
├── CLAUDE.md                    ← your brain's operating manual
├── second-brain-intake.md       ← your answers (editable; re-run the skill to update)
├── function-inventory.md        ← audit template (used on Day 2 of the bootcamp)
├── context/
│   ├── about-me.md
│   ├── about-business.md
│   ├── services.md
│   ├── icp.md
│   ├── priorities.md
│   └── never-assume.md
└── references/
    ├── voice.md
    └── voice-notes.md (if you pasted writing samples)
```

After running `/hire` you'll also have:

```
my-brain/
└── employees/
    └── <name>.md                ← your first AI employee's JD
```

Your AI employee comes alive on Day 3 of the bootcamp. To call them into a chat, just address them by name. Saying *"Hi Cleo, what should I focus on?"* causes Claude to read `employees/cleo.md`, adopt that identity, and respond as Cleo. Switching employees is just switching names. One brain, many employees, all in the same project.

---

## How to iterate

Both skills are **idempotent**. You can re-run them as your business changes.

- Edit `second-brain-intake.md` (your answers), re-run `/second-brain`, and the brain regenerates. Previous versions back up to `archives/`.
- Run `/hire` again with a different name to add a second employee. Same name twice creates `<name>-2.md`, not overwrite. All employees live in the same project and you switch between them by addressing them by name.

You drive the brain by editing answers in the intake file. The skill does the file-writing.

---

## Licence

MIT. Use it, fork it, ship it under your own brand.

---

*Built for the Chofski Consulting "Build Your Second Brain with Claude" bootcamp. Question set modelled on Nate Herk's `/onboard` pattern from AIS-OS, retuned for creative founders without a connectable tooling stack.*
