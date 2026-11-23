# PRD Generator skill for Claude Code, Codex and Cursor

A free agent skill that turns a rough idea into a short, screen-ready PRD (product requirements document) that an AI app builder, a coding agent or a designer can build from. Next to the decision and scope, it lists every screen, what each one shows in every state, the words on it and how to check it is done. It works in Claude Code, Codex, Cursor and any agent that supports skills.

## Install

```bash
npx skills add uxpilot-ai/prd-generator-skill
```

Or copy the `skills/prd-generator` folder into your agent's skills folder (for Claude Code, `~/.claude/skills/`).

## What it does

- Sizes the document to the job: three lines for a small change, a page or two for an MVP.
- Asks up to five quick questions with suggested answers, or drafts at once when you say "just write it", listing every assumption it made.
- Lists every screen with its purpose, what it shows in order of importance and its actions.
- Covers each screen's first use, empty, loading, error and success states, with the exact words people will read.
- Writes non-goals, rules and limits as exact numbers, done checks, and a build order you can hand over one slice at a time.
- Decides what each screen says and does, and leaves how it looks to your designer or design tool.

## Example prompts

- "Write a PRD for a habit tracker for remote teams. Just write it."
- "Turn these notes into a PRD I can paste into my app builder."
- "Here are screenshots of our app. Write a PRD for adding team invites."
- "Write the PRD for an MVP of a booking tool for yoga studios."

## What's inside

| File | What it covers |
|---|---|
| `SKILL.md` | Sizing the document, when to ask and when to draft, the final checks |
| `references/prd-template.md` | The PRD, part by part, with notes on each part |
| `references/states-and-words.md` | The five screen states, the words on screen, and one worked screen |

## Made by UX Pilot

[UX Pilot](https://uxpilot.ai/?utm_source=prd-generator&utm_medium=readme) is an AI UI design tool. It can design the screens in your PRD, user flows and clickable prototypes, and check them with a UX review.

## License

[Apache License 2.0](LICENSE): use, change and share it freely. Keep the [NOTICE](NOTICE) file when you do.
