# Clean Comms

![Clean Comms banner — Few, short messages for any AI agent](<https://ghrb.waren.build/render/banner?header=Clean+Comms&subheader=Few%2C+short+messages+for+any+AI+agent&bg=1C2430-3D5A73&color=FFFFFF&subheadercolor=E4EEF6&headerfont=DM+Sans&subheaderfont=Inter&support=true&watermarkpos=bottom-right>)
<!-- Created with GitHub Repo Banner by Waren Gonzaga: https://ghrb.waren.build -->

[![License: MIT](https://img.shields.io/badge/license-MIT-3D5A73)](LICENSE)

**Clean Comms** is a generic skill that teaches an AI agent to talk to its user in short, clear messages.

It is for anyone whose agent can load an Agent Skills folder. Talking to the agent should feel like chatting with a person. The agent sends few messages. It adds detail only when the user asks.

[Skill rules](skills/clean-comms/SKILL.md) · [Repository instructions](AGENTS.md)

## ✨ Features

- **Short by default.** A reply is one or two lines. The answer, result, or question is in the first line.
- **One message per update.** The agent writes for a result, a decision you must make, or a blocker. It does not narrate progress.
- **No extra information.** It does not restate the task, explain its process, or add options you did not ask for.
- **Plain detail when you ask.** A longer answer waits for a request such as "detailed", "explain", or a full document.
- **Your language and register.** The agent matches how you write, including mixed language, without making the reply longer.

## 🚀 Getting Started

You need an agent host that loads a skill from a folder containing `SKILL.md`. This repository has no package to install and no plugin manifest, so there is no marketplace command.

1. Copy `skills/clean-comms/` into the skills directory your host already uses.
2. Start a new session so the host loads the skill. Its name is `clean-comms`.

Ask a short status question. The first useful result is a one- or two-line answer, with the result in the first line.

## 📖 Usage

After the skill is loaded, a normal update stays short. The skill's own example of a finished update is:

```text
Button renamed. Tests passed.
```

That sample shows the reply shape. It is not a test result from this repository. The agent does not first send "On it." and then recap the same work.

If one extra detail would help, the agent may add one short offer:

```text
Button renamed. I can show the diff.
```

A long message is for an explicit request, such as "explain" or "detailed", or for a full document. Until then, the reply stays short. The same limit applies in every language.

### What the agent leaves out

The agent does not restate your request. It leaves out logs, tool names, and side facts unless you need them to act. In chat it does not add headers, tables, or a list longer than three short bullets unless you ask.

## 📚 Documentation

- [clean-comms skill](skills/clean-comms/SKILL.md): the rules, limits, and good and bad examples.
- [Repository instructions](AGENTS.md): how to change this repository without widening its scope.

This repository does not include a plugin guide, changelog, or release workflow.

## 🛠️ Development

There is no application build and no automated test suite.

For a documentation or skill change:

1. Inspect the diff and run `git diff --check`.
2. Check that relative Markdown links resolve.
3. Check that the frontmatter `name` in `skills/clean-comms/SKILL.md` is `clean-comms`.

[AGENTS.md](AGENTS.md) is the full contributor checklist.

## 🤝 Contributing

Documentation and skill fixes are welcome. Read [AGENTS.md](AGENTS.md) before you open a pull request.

- Create a short-lived branch from `dev`.
- Open the pull request against `dev`.
- Do not push directly to `dev` or `main` for routine changes.
- Promote `dev` to `main` only when a maintainer has authorized it.
- Use [Clean Commit](https://github.com/wgtechlabs/clean-commit) messages: `<emoji> <type>: <description>`, in lowercase present tense, with no final period.

Keep the skill generic. Do not add a plugin manifest, release workflow, or sync script unless a maintainer asks for it.

## 🐛 Issues & Support

Search [existing issues](https://github.com/wgtechlabs/clean-comms/issues) before you open a [new issue](https://github.com/wgtechlabs/clean-comms/issues/new).

For a skill question, include the behavior you expected and a short example of the message. Do not include credentials, private logs, or other secrets.

This repository has no separate security-reporting policy and no private support address.

## 📄 License

Clean Comms is licensed under the [MIT License](LICENSE).

Copyright (c) 2026 WG Technology Labs.

## 👥 Authors & Contributors

Created by **[Waren Gonzaga](https://github.com/warengonzaga)** under **[WG Technology Labs](https://github.com/wgtechlabs)**, with contributions from the [community](https://github.com/wgtechlabs/clean-comms/graphs/contributors).
