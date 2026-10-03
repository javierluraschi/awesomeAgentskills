# Cloudish

Deploy an app to [Cloudish](https://cloudish.ai) and get back a live URL. The agent
inspects the project, uses an existing Dockerfile or writes a minimal one, creates its
own API key if needed, deploys, and reports the URL. Cloudish builds the image
server-side, so no local Docker is required.

`SKILL.md` here is a copy of the upstream skill at
[cloudishai/skills](https://github.com/cloudishai/skills/tree/main/skills/cloudish)
(MIT, see `LICENSE`). It tells the agent to read https://cloudish.ai/skill.md for
the current API before making any call.

## Install

```bash
mkdir -p ~/.claude/skills/cloudish
cp SKILL.md ~/.claude/skills/cloudish/
```

Or install it as a Claude Code plugin:

```
/plugin marketplace add cloudishai/skills
/plugin install cloudish@cloudishai
```

Then ask your agent: *"Deploy this app to Cloudish."*
