# skills

Personal collection of agent skills in `SKILL.md` format.

## Skills

| Skill | Purpose | Files |
|---|---|---|
| [`technical-writing-style`](technical-writing-style/SKILL.md) | Rules, acceptance criteria, and verification steps for drafting, revising, and reviewing technical and explanatory prose, distilled from Laplante's *Technical Writing* and reader-centred editing practice. | [SKILL.md](technical-writing-style/SKILL.md), [reference.md](technical-writing-style/reference.md) |

## Installation

Clone the repository and symlink or copy any skill directory into your agent's skills directory (for example, `~/.agents/skills/`):

```bash
git clone git@github.com:k-soomro/skills.git
ln -s "$(pwd)/skills/technical-writing-style" ~/.agents/skills/technical-writing-style
```

## Skill structure

Each skill lives in its own top-level directory containing at least a `SKILL.md` file with YAML frontmatter:

```markdown
---
name: skill-name
description: When to trigger the skill and what it covers.
---
```

Supporting material (such as extended word lists, templates, or scripts) belongs alongside `SKILL.md` in the same directory (for example, [`technical-writing-style/reference.md`](technical-writing-style/reference.md)).
