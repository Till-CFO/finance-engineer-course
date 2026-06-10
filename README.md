# The Finance Engineer Course

A hands-on Claude Code course for finance, ops, and admin professionals. No technical background needed — if you can write an email, you can do this course.

Six interactive modules (plus a bonus), each taught *by Claude, inside Claude Code*. You don't read about the tool — the tool teaches you, using realistic finance-team work: messy Slack threads, half-written emails, raw meeting notes, a general ledger with problems hidden in it.

Built by the team at [Till CFO](https://tillcfo.com), who run their finance services firm on these exact patterns.

> **Note:** Every company and person in the course scenarios — Meridian Finance Partners, Brightline Ventures, and everyone who works there — is fictional. That's deliberate: you practice on realistic material without anyone's real data.

## What's Inside

| Module | What you'll do | Time |
|--------|----------------|------|
| 1 — Your First Day | Get comfortable; turn a messy Slack thread into action items; rescue a bad email draft | ~20 min |
| 2 — Communications Superpower | Triage an inbox; draft replies in your own voice | ~25 min |
| 3 — Meeting Machine | Prep briefs from thin calendar invites; turn raw notes into decisions + action items | ~25 min |
| 4 — Your Daily Patterns | Prioritize a real Monday task list; build your daily rhythm | ~30 min |
| 5 — Build Your OS | The capstone: your own workspace, memory file, writing voice, and first connected tool | ~40 min |
| 6 — The Finance Lens | Run an open-ended analysis on a general ledger and watch Claude find what's hidden in it | ~25 min |
| Bonus — Going Deeper | Shortcuts, helpers, and where to take it next | self-paced |

Also included:

- **`/gl-review`** — a finished, reusable skill that runs a first-pass review on any GL export (duplicates, miscodings, recognition flags, spikes). It's the Module 6 exercise, productized — and a working example of what you'll be able to build yourself after Module 5.
- **[What You Can Build](plugins/finance-engineer-course/WHAT-YOU-CAN-BUILD.md)** — a catalog of the patterns the Till CFO team runs internally, as inspiration for your own builds.

## Getting Started

There are two ways to run the course. **Pick one** — the course itself is identical in both.

### Path A — Claude Code desktop app (recommended for most people)

No terminal involved.

1. Download the **Claude Code desktop app** for Mac or Windows from [claude.com/claude-code](https://claude.com/claude-code) and sign in with your Claude account.
2. Open the app and choose a folder to work in — your Documents folder is fine.
3. Paste these two lines (one at a time) into the message box:

```
/plugin marketplace add <ORG>/finance-engineer-course
/plugin install finance-engineer-course@finance-engineer-course
```

4. Then type:

```
/start-1-1
```

Claude takes it from there. Each module ends by pointing you to the next one.

### Path B — Terminal

If you're comfortable in a terminal (or just curious). Never opened one? Use the **[step-by-step terminal walkthrough](terminal-setup.html)** — about 5 minutes, written for people who've never seen a blinking cursor.

The short version:

1. Install the **Claude Code CLI** per the instructions at [claude.com/claude-code](https://claude.com/claude-code), then confirm it runs: open a terminal and type `claude`.
2. From any folder you'd like to work in (Documents is fine), type `claude`, then run the same three commands as Path A: the two `/plugin` lines, then `/start-1-1`.

### Either path

To get course updates later: `/plugin marketplace update finance-engineer-course`.

**Prefer not to use plugins?** Clone (or download) this repo, open the repo folder — in the desktop app, or in a terminal with `claude` — and run `/start-1-1`. Everything works the same.

## Questions / Feedback

Open an issue on this repo — we read them.

## License

See [LICENSE.md](LICENSE.md). You're welcome to take the course, share it with your team, and build on what you learn. Please don't resell or commercially redistribute the course materials themselves.
