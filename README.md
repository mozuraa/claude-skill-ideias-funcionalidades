# Ideias de funcionalidades · Feature ideas — Claude Skill

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
![Claude Skill](https://img.shields.io/badge/Claude-Skill-D97757)

📚 Faz parte da **[biblioteca de skills de mozuraa](https://github.com/mozuraa/claude-skills)** · Part of **[mozuraa's skills library](https://github.com/mozuraa/claude-skills)**

**🇬🇧 English · [🇵🇹 Português](README.pt.md)**

---


A [skill](#what-is-a-skill) for **Claude** (Claude Code, the Claude app and claude.ai).

### What it does

Generates **2–3 well-developed new features** for an app or game that **already exists** — game modes, levels, power-ups, screens, retention improvements. Before suggesting anything, Claude takes a quick look at the app's code so it doesn't propose what's already there and can say exactly which files each idea touches.

### When it triggers

Claude uses it on its own when you ask things like:

- "What can I add to my game?"
- "How do I make my app more engaging?"
- "Ideas for a new game mode"
- "Users quit after a week — what's missing?"

You can also call it directly with `/ideias-funcionalidades`.

### What you get

Every idea always includes:

- What it is
- Why it's worth it
- How it fits the app (with real file names)
- Design details (rules and numbers)
- Effort
- How to tell if it worked

At the end, Claude says which one it recommends and why, and offers to go deeper.

See a full example in [`examples/exemplo.md`](examples/exemplo.md) (in Portuguese).

### Details

- Works best when Claude can see the code (Claude Code, inside the project folder).
- With no code or context, it asks a single question: a one-sentence description of the app.
- Checks in the code that whatever an idea depends on actually exists before proposing it.
- Replies in the language you write in — the instructions are in Portuguese, but it works in any language.

### Installation

**Claude Code (all your projects)**

```bash
git clone https://github.com/mozuraa/claude-skill-ideias-funcionalidades.git ~/.claude/skills/ideias-funcionalidades
```

**Claude Code (one project only)** — from the project folder:

```bash
git clone https://github.com/mozuraa/claude-skill-ideias-funcionalidades.git .claude/skills/ideias-funcionalidades
```

Start a new session so the skill is loaded.

**Claude app / claude.ai**

1. On this page, click **Code → Download ZIP**.
2. In Claude, open **Settings** and find the **Skills** section (under *Capabilities*).
3. Upload the ZIP. The skill becomes available in your chats.

> Custom skills must be enabled for your account/organization.

### Updating

```bash
cd ~/.claude/skills/ideias-funcionalidades && git pull
```

### What is a skill?

A skill is a folder with a `SKILL.md` file: a name, a description of when it should be used, and instructions. Claude only reads the description until it becomes relevant; when a request matches, it loads the instructions and follows them. It installs no programs and runs no code — it's just text.

### Structure

```
claude-skill-ideias-funcionalidades/
├── SKILL.md            # the skill (name, description and instructions)
├── examples/
│   └── exemplo.md      # example request and answer
├── README.md · README.pt.md
├── CHANGELOG.md
└── LICENSE
```

### Idea skills family

| Skill | What for |
|---|---|
| [`app-studio`](https://github.com/mozuraa/claude-skill-app-studio) | Apps: ideate, create and diagnose |
| [`ideias-funcionalidades`](https://github.com/mozuraa/claude-skill-ideias-funcionalidades) *(this one)* | Feature ideas |
| [`ideias-monetizacao`](https://github.com/mozuraa/claude-skill-ideias-monetizacao) | Monetization ideas |
| [`brainstorming`](https://github.com/mozuraa/claude-skill-brainstorming) | Brainstorming |

### Contributing

Suggestions and improvements are welcome: open an issue or a pull request. If the skill didn't trigger when it should have (or did when it shouldn't), share the prompt — it helps tune the description.

### License

[MIT](LICENSE) — free to use, modify and share, keeping the license notice.
