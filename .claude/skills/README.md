# Skills

These 25 skills are vendored from [mattpocock/skills](https://github.com/mattpocock/skills)
(MIT, © Matt Pocock — see `LICENSE-mattpocock-skills`), v1.2.2.

**Engineering:** ask-matt, code-review, codebase-design, diagnosing-bugs, domain-modeling,
grill-with-docs, implement, improve-codebase-architecture, prototype, research,
resolving-merge-conflicts, setup-matt-pocock-skills, tdd, to-spec, to-tickets, triage,
wayfinder, wizard

**Productivity:** grill-me, grilling, handoff, teach, to-questionnaire, wait-what,
writing-for-agents

## Usage

Invoke by name, e.g. `/grill-me`, `/wait-what`, `/to-tickets`.

Run `/setup-matt-pocock-skills` once in this repo first — it configures the issue tracker,
triage labels, and docs layout the other skills expect.

## Updating

```sh
git clone --depth 1 https://github.com/mattpocock/skills.git /tmp/mp-skills
cp -r /tmp/mp-skills/skills/engineering/* /tmp/mp-skills/skills/productivity/* .claude/skills/
```

Alternatively, install as a managed plugin instead of vendoring:
`/plugin install mattpocock-skills`.
