# Ideias de funcionalidades · Feature ideas — Claude Skill

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
![Claude Skill](https://img.shields.io/badge/Claude-Skill-D97757)

**[Português](#português) · [English](#english)**

---

## Português

Uma [skill](#o-que-é-uma-skill) para o **Claude** (Claude Code, app Claude e claude.ai).

### O que faz

Gera **2 a 3 funcionalidades novas, bem desenvolvidas**, para uma app ou jogo que **já existe** — modos de jogo, níveis, power-ups, ecrãs, melhorias de retenção. Antes de propor, o Claude dá uma vista de olhos rápida ao código da app para não sugerir o que já está feito e para dizer exatamente em que ficheiros cada ideia encaixa.

### Quando é ativada

O Claude usa-a sozinho quando pedes algo como:

- "O que posso adicionar ao meu jogo?"
- "Como torno a minha app mais viciante?"
- "Ideias para um modo novo"
- "Os utilizadores desistem ao fim de uma semana, o que falta?"

Também a podes chamar diretamente com `/ideias-funcionalidades`.

### O que recebes

Cada ideia vem sempre com:

- O que é
- Porque vale a pena
- Como encaixa na app (com nomes de ficheiros reais)
- Detalhes de design (regras e números)
- Esforço
- Como testar se resultou

No fim, o Claude diz qual recomenda e porquê, e oferece-se para aprofundar.

Vê um exemplo completo em [`examples/exemplo.md`](examples/exemplo.md).

### Detalhes

- Funciona melhor quando o Claude tem acesso ao código (Claude Code, numa pasta do projeto).
- Sem código nem contexto, faz uma única pergunta: uma descrição da app numa frase.
- Confirma no código que aquilo de que uma ideia depende existe mesmo, antes de a propor.
- Responde na língua em que escreves — as instruções estão em português, mas funciona em qualquer língua.

### Instalação

**Claude Code (para todos os teus projetos)**

```bash
git clone https://github.com/mozuraa/claude-skill-ideias-funcionalidades.git ~/.claude/skills/ideias-funcionalidades
```

**Claude Code (só num projeto)** — dentro da pasta do projeto:

```bash
git clone https://github.com/mozuraa/claude-skill-ideias-funcionalidades.git .claude/skills/ideias-funcionalidades
```

Abre uma sessão nova para a skill ser carregada.

**App Claude / claude.ai**

1. Nesta página, carrega em **Code → Download ZIP**.
2. No Claude, abre as **Definições** e procura a secção **Skills** (em *Capacidades*).
3. Carrega o ZIP. A skill fica disponível nas tuas conversas.

> As skills personalizadas precisam de estar ativadas na tua conta/organização.

### Atualizar

```bash
cd ~/.claude/skills/ideias-funcionalidades && git pull
```

### O que é uma skill?

Uma skill é uma pasta com um ficheiro `SKILL.md`: um nome, uma descrição de quando deve ser usada e instruções. O Claude lê só a descrição até ela ser útil; quando o pedido encaixa, carrega as instruções e segue-as. Não instala programas nem corre código — é só texto.

### Estrutura

```
claude-skill-ideias-funcionalidades/
├── SKILL.md            # a skill (nome, descrição e instruções)
├── examples/
│   └── exemplo.md      # exemplo de pedido e resposta
├── README.md
├── CHANGELOG.md
└── LICENSE
```

### Família de skills de ideias

| Skill | Para quê |
|---|---|
| [`ideias-apps`](https://github.com/mozuraa/claude-skill-ideias-apps) | Ideias de apps e jogos |
| [`ideias-funcionalidades`](https://github.com/mozuraa/claude-skill-ideias-funcionalidades) *(esta)* | Ideias de funcionalidades |
| [`ideias-monetizacao`](https://github.com/mozuraa/claude-skill-ideias-monetizacao) | Ideias de monetização |
| [`brainstorming`](https://github.com/mozuraa/claude-skill-brainstorming) | Brainstorming |

### Contribuir

Sugestões e melhorias são bem-vindas: abre uma *issue* ou um *pull request*. Se a skill não se ativou quando devia (ou ativou quando não devia), diz qual foi o pedido — ajuda a afinar a descrição.

### Licença

[MIT](LICENSE) — podes usar, alterar e partilhar livremente, mantendo o aviso de licença.

---

## English

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

### Idea skills family

| Skill | What for |
|---|---|
| [`ideias-apps`](https://github.com/mozuraa/claude-skill-ideias-apps) | App & game ideas |
| [`ideias-funcionalidades`](https://github.com/mozuraa/claude-skill-ideias-funcionalidades) *(this one)* | Feature ideas |
| [`ideias-monetizacao`](https://github.com/mozuraa/claude-skill-ideias-monetizacao) | Monetization ideas |
| [`brainstorming`](https://github.com/mozuraa/claude-skill-brainstorming) | Brainstorming |

### Contributing

Suggestions and improvements are welcome: open an issue or a pull request. If the skill didn't trigger when it should have (or did when it shouldn't), share the prompt — it helps tune the description.

### License

[MIT](LICENSE) — free to use, modify and share, keeping the license notice.
