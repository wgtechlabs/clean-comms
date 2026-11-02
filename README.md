# Clean Comms

A generic skill that teaches an AI agent to talk to its user in short, clear messages.

Talking to the agent should feel like chatting with a person.
The agent sends few messages.
It does not add extra information unless the user asks.

## Install

Agents that support the Agent Skills format can load this folder directly:

```text
skills/clean-comms/
```

Copy `skills/clean-comms/` into the skills path your agent already uses.
The folder name and the skill name are both `clean-comms`.

## What the skill covers

The skill keeps user-facing chat short.

- One or two lines by default. The answer comes first.
- One message per update. No progress play-by-play.
- No extra detail, options, or tutorials unless the user asks.
- Plain technical writing when a longer answer is requested.
- The user's language and register, without writing more.

Read [skills/clean-comms/SKILL.md](skills/clean-comms/SKILL.md) for the rules and examples.

## Contributing

Create a short-lived branch from `dev`.
Open the pull request against `dev`.
Use [Clean Commit](https://github.com/wgtechlabs/clean-commit) messages.
See [AGENTS.md](AGENTS.md) for repository instructions.

## License

MIT. See [LICENSE](LICENSE).
