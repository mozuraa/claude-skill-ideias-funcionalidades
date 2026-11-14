# Ideias de funcionalidades · Feature ideas — Claude Skill

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
![Claude Skill](https://img.shields.io/badge/Claude-Skill-D97757)

📚 Faz parte da **[biblioteca de skills de mozuraa](https://github.com/mozuraa/claude-skills)** · Part of **[mozuraa's skills library](https://github.com/mozuraa/claude-skills)**

**[🇬🇧 English](README.md) · 🇵🇹 Português**

---


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
├── README.md · README.pt.md
├── CHANGELOG.md
└── LICENSE
```

### Família de skills de ideias

| Skill | Para quê |
|---|---|
| [`app-studio`](https://github.com/mozuraa/claude-skill-app-studio) | Apps: idear, criar e diagnosticar |
| [`ideias-funcionalidades`](https://github.com/mozuraa/claude-skill-ideias-funcionalidades) *(esta)* | Ideias de funcionalidades |
| [`ideias-monetizacao`](https://github.com/mozuraa/claude-skill-ideias-monetizacao) | Ideias de monetização |
| [`brainstorming`](https://github.com/mozuraa/claude-skill-brainstorming) | Brainstorming |

### Contribuir

Sugestões e melhorias são bem-vindas: abre uma *issue* ou um *pull request*. Se a skill não se ativou quando devia (ou ativou quando não devia), diz qual foi o pedido — ajuda a afinar a descrição.

### Licença

[MIT](LICENSE) — podes usar, alterar e partilhar livremente, mantendo o aviso de licença.
