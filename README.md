# Vue Reviewer

**English** | [Português (Brasil)](README.pt-BR.md)

An agent skill that reviews **Vue 3** frontends (Vite SPA or Nuxt) and **@nuxt/ui**.

It identifies the project's real framework and flags APIs from the wrong framework, routing/guard issues, misuse of the HTTP client, and composable and reactivity anti-patterns.

The skill is **read-only**: it analyzes and reports without editing files.

It follows the open [Agent Skills](https://agentskills.io) format (`SKILL.md` with `name` and `description` frontmatter) and works with Claude Code, Cursor and other compatible agents. The skill instructions are written in Brazilian Portuguese.

## Installation

The target folder must be named `vue-reviewer` (the skill name), not the repository name.

### Claude Code

```bash
# All projects
git clone https://github.com/jrcarls/skill-vue-reviewer.git ~/.claude/skills/vue-reviewer

# A single project
git clone https://github.com/jrcarls/skill-vue-reviewer.git .claude/skills/vue-reviewer
```

### Cursor

```bash
git clone https://github.com/jrcarls/skill-vue-reviewer.git .cursor/skills/vue-reviewer
```

## Usage

The agent loads the skill automatically when the task matches its description. To invoke it explicitly in Claude Code:

```text
/vue-reviewer
```

## Related skills

This skill is part of a complementary set:

- `skill-owasp-security-reviewer` — OWASP Top 10
- `skill-llm-security-reviewer` — OWASP LLM Top 10
- `skill-tenant-isolation-reviewer` — IDOR / ownership
- `skill-lgpd-compliance-advisor` — LGPD compliance
- `skill-qa-verifier` — functional verification
- `skill-vue-reviewer` — Vue frontend review

## License

[MIT](LICENSE)
