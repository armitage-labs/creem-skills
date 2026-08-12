# CREEM Skills for AI Coding Assistants

> [!IMPORTANT]
> **This repository is a pointer.** The Creem skill is now maintained in
> **[armitage-labs/creem](https://github.com/armitage-labs/creem)** at
> [`packages/docs/skills/creem-api`](https://github.com/armitage-labs/creem/tree/main/packages/docs/skills/creem-api),
> alongside the SDKs and the API docs, so it can never drift from the platform again.
>
> This repo now contains only a marketplace manifest that resolves to that folder.
> **Nothing here needs editing** — open skill changes against `armitage-labs/creem`.

Official Creem payment integration skills for AI coding assistants like Claude Code, Cursor, and Windsurf.

## Install (Claude Code)

Nothing changes if you already installed from here — run `/plugin marketplace update creem-skills` and you will pick up the maintained skill automatically.

New installs should use the canonical source:

```bash
/plugin marketplace add armitage-labs/creem
/plugin install creem-api@creem-skills
```

The older `/plugin marketplace add armitage-labs/creem-skills` still works and resolves to the same files.

## Install (Cursor, Windsurf, and other tools)

Pull just the skill folder into your project:

```bash
npx degit armitage-labs/creem/packages/docs/skills/creem-api .cursor/skills/creem-api
```

Then reference it in conversation:

```
@.cursor/skills/creem-api/SKILL.md Help me create a checkout flow
```

## What's in the skill

| File           | Description                                                 |
| -------------- | ----------------------------------------------------------- |
| `SKILL.md`     | Core skill with quick reference and implementation patterns |
| `REFERENCE.md` | Complete API reference with all endpoints and schemas       |
| `WEBHOOKS.md`  | Webhook events documentation with payload examples          |
| `WORKFLOWS.md` | Step-by-step integration guides for common use cases        |

## Documentation

- Skill setup guide: https://docs.creem.io/code/sdks/ai-agents
- API documentation: https://docs.creem.io

## License

MIT
