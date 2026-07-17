# skills

A collection of agent skills. Each top-level folder is a self-contained skill with a `SKILL.md` and, where needed, a `references/` directory.

## Install

Install skills from this repo with the [`skills`](https://www.npmjs.com/package/skills) CLI. You can run it ad hoc via `npx skills`, no install required — every example below uses this form.

Optionally, install the CLI itself globally so you can just call `skills` instead of `npx skills`:

```bash
npm install -g skills
```

Add all skills from this repo to your project:

```bash
npx skills add devioarts/skills
```

Add a specific skill to a specific agent:

```bash
# Claude Code
npx skills add devioarts/skills --skill <skill-name> -a claude-code

# Codex
npx skills add devioarts/skills --skill <skill-name> -a codex
```

Install to your user/global skills directory instead of the current project:

```bash
# Claude Code
npx skills add devioarts/skills --skill <skill-name> -g -a claude-code

# Codex
npx skills add devioarts/skills --skill <skill-name> -g -a codex
```

List the skills available in this repo before installing:

```bash
npx skills add devioarts/skills --list
```

Update installed skills to the latest version:

```bash
# update everything installed from this repo
npx skills update devioarts/skills

# update a single skill
npx skills update <skill-name>
```

Other useful commands once skills are installed:

```bash
npx skills list                       # show installed skills
npx skills remove <skill-name>        # uninstall a skill
```

See the [`skills` CLI documentation](https://www.npmjs.com/package/skills) for the full list of supported agents and flags.

## Manual install

You can also copy a skill folder directly into your agent's skills directory. Keep the whole folder together (including `references/`).

- Claude Code (personal): `~/.claude/skills/<skill-name>`
- Claude Code (project-local): `.claude/skills/<skill-name>`
- Codex (personal): `~/.codex/skills/<skill-name>`
- Codex (project-local): `.agents/skills/<skill-name>`

## License

MIT — see [LICENSE](LICENSE).
