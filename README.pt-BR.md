# Vue Reviewer

[English](README.md) | **Português (Brasil)**

Skill de agente para revisão de frontends **Vue 3** (SPA com Vite ou Nuxt) e **@nuxt/ui**.

Identifica o framework real do projeto e aponta APIs do framework errado, falhas de roteamento/guards, uso incorreto do cliente HTTP, anti-padrões de composables e reatividade.

A skill é **somente leitura**: analisa e reporta, sem editar arquivos.

Segue o formato aberto de [Agent Skills](https://agentskills.io) (`SKILL.md` com frontmatter `name` e `description`) e funciona no Claude Code, Cursor e outros agentes compatíveis.

## Instalação

A pasta de destino deve se chamar `vue-reviewer` (o nome da skill), não o nome do repositório.

### Claude Code

```bash
# Para todos os projetos
git clone https://github.com/jrcarls/skill-vue-reviewer.git ~/.claude/skills/vue-reviewer

# Apenas para um projeto
git clone https://github.com/jrcarls/skill-vue-reviewer.git .claude/skills/vue-reviewer
```

### Cursor

```bash
git clone https://github.com/jrcarls/skill-vue-reviewer.git .cursor/skills/vue-reviewer
```

## Uso

O agente carrega a skill automaticamente quando a tarefa combina com a descrição. Para chamar explicitamente no Claude Code:

```text
/vue-reviewer
```

## Skills relacionadas

Esta skill faz parte de um conjunto que se complementa:

- `skill-owasp-security-reviewer` — OWASP Top 10
- `skill-llm-security-reviewer` — OWASP LLM Top 10
- `skill-tenant-isolation-reviewer` — IDOR / ownership
- `skill-lgpd-compliance-advisor` — conformidade LGPD
- `skill-qa-verifier` — verificação funcional
- `skill-vue-reviewer` — revisão de frontend Vue

## Licença

[MIT](LICENSE)
