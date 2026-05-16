# agent-skeleton

Skeleton body for a production agent: a `SKILL.md` template with 13 structural blocks, a self-check checklist, and a filled example.

[Русская версия](./README.md)

## What is this

This is a companion repository to the article "Anatomy of a production agent 2026: analysis of two open Anthropic prompts" (in Russian). The article analyzes two production prompts from `anthropics/claude-cookbooks`, extracts 13 structural blocks that should live in any working agent, and assembles a `SKILL.md` template for adaptation.

This repository contains the full template, a checklist, and a working example. To assemble your own agent, clone the repository, open `SKILL.md`, walk through the placeholders, and adapt to your task.

## What's inside

- **`SKILL.md`** — main template with placeholders and explanations for each block. This is the file you adapt to your task.
- **`CHECKLIST.md`** — a checklist of 13 blocks for self-checking your finished agent.
- **`examples/research-agent/`** — filled example: a research agent that gathers facts from the web and internal sources.
- **`docs/how-to-use.md`** — short instructions on how to connect the skill to Claude.ai and Claude Code.

## Quick start

1. Clone or download the repository.
2. Open `SKILL.md` and walk through it top to bottom, replacing placeholders to fit your task.
3. Cross-check with `CHECKLIST.md` — are all 13 blocks filled in.
4. Connect the finished skill to your agent (see `docs/how-to-use.md`).

## 13 skeleton blocks

1. Agent role and goal
2. Current date
3. Task type (request classification)
4. Research process (explicit work phases)
5. OODA loop (reflection after each step)
6. Research budget (soft tool-call budget)
7. Parallel tool calls
8. Tool selection (explicit list with descriptions)
9. Internal tools priority
10. Source quality (data quality criteria)
11. Maximum tool call limit (hard resource ceiling)
12. Output formatting (completion format)
13. Synthesis responsibility (role separation in multi-agent systems)

## Why the template is in English

Claude was trained on a mixed-language corpus, but the density of agent-related instructions in it is highest in English. Russian system prompts work, but they give noticeably worse metrics on long reasoning chains.

All production prompts that Anthropic releases publicly are in English. Their own system prompts for Claude.ai, Claude Code, and Claude Research are in English too.

Practical tip: if your agent's interface is in another language (a bot, web form, internal tool) — translate only what the user sees in the final output. Keep system instructions, tool descriptions, and task classifiers in English.

## Contributing

Pull requests are welcome. If you find something to improve in the template, or want to add your own example — open an issue or send a PR directly.

## Author

Vitaly Turyev — Lead Product Designer, article series on production agents in 2026.

- Telegram: [«Я и мой друг робот»](https://t.me/mewithrobot)

## License

[MIT](./LICENSE) — use freely in personal and commercial projects.
