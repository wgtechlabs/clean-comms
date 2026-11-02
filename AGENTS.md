# Repository instructions

## Scope

This repository distributes the `clean-comms` skill.
The canonical instructions are in `skills/clean-comms/SKILL.md`.
Keep the skill generic. Do not add owner names, product names, or a required user language.
Mixed-language examples, such as Taglish, show a pattern. They are not a default language.
Read the current skill before changing behavior.
Keep edits limited to the requested outcome.

The skill teaches an agent to talk like a person.
Short messages are the default.
Extra detail belongs in the skill only when a rule needs it to be usable.

## Documentation

- Keep the skill folder and the frontmatter `name` as `clean-comms`.
- Update the README when install steps or skill behavior change.
- Preserve the MIT license.
- Do not add a plugin manifest, release workflow, or sync script unless asked.

## Git and delivery

- Create short-lived branches from `dev`.
- Open pull requests against `dev`.
- Do not push directly to `dev` or `main` for routine changes.
- Promote `dev` to `main` only when authorized.
- Use Clean Commit messages: `<emoji> <type>: <description>`.
  Use lowercase, present-tense descriptions. Do not add a final period.
  Common pairs are `📖 docs`, `📦 new`, `🔧 update`, `⚙️ setup`, and `🧪 test`.

## Validation

For skill or documentation changes, inspect the diff and run `git diff --check`.
Check that relative Markdown links resolve.
Check that the frontmatter `name` matches the skill folder.
