# build-on-what-worked

**Your agent starts from the piece that already worked, meets every point it had, beats it on at least one, and shows you the side-by-side.**

`build-on-what-worked` is an agent skill for Claude Code (and any agent that reads `SKILL.md` skills). It is for agencies and freelancers who make the same kinds of things for many clients: websites, landing pages, proposals, ad videos, campaigns.

Without it, an agent asked for "a site for the new client" tends to:
- start from a blank page when a proven site for the same niche already exists;
- ship fewer sections, a missing conversion tag or a weaker call to action than last time;
- deliver a "version 1" with "the rest later";
- say "done" without comparing against anything.

This skill gives it:
- **A proven base first.** It searches past work for something that worked or that the owner approved, and builds on it. It starts from zero only when the owner asks for something new, or nothing similar exists.
- **A checklist from the base.** Every point the base had gets a check in the new piece, plus at least one concrete improvement.
- **No 50% deliveries.** No "version 1", no empty sections, no placeholders. When a fact or a third party is missing, everything else gets done and the gap goes in one line.
- **A side-by-side table** with the delivery, each check verified on the real result.
- **Brand kept apart.** It reuses the structure that sells, never the look. Two clients do not end up identical.

## Install

```bash
npx skills add RabbitDesigns22/build-on-what-worked
```

Or copy `skills/build-on-what-worked/` into `~/.claude/skills/`.

## Works well with

- [`do-it-now`](https://github.com/RabbitDesigns22/do-it-now), to start the order in the same turn.
- A verification skill, such as `verification-before-completion`, to check the result before saying "done".

## Status and limits

Version 1. It comes from the author's agency work. A new client's site was designed from zero, while a proven site for the same niche, with ads converting, was already there. The owner asked for "no more half-done work".

- It only finds what is in the folders the agent can read. Keep past work and approvals where it can find them.
- "Worked" means a result or an approval you can point to, not a feeling. If nothing qualifies, the skill says so and starts fresh.

MIT. Issues welcome.
