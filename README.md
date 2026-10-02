# Kiliaan Vanvoorden

Self-taught engineer. I build the verification layer for AI systems — the gates, tests and
CI that decide whether a system is actually right, and that fail loudly when it isn't.

**Open to AI engineering roles where the evaluation harness _is_ the job.** Available
immediately, EU citizen based in Riemst, Belgium — no work sponsorship required, and able to
work remotely for EU or US employers.

- Email: [bakerstreetbandit@zohomail.eu](mailto:bakerstreetbandit@zohomail.eu)
- GitHub: [github.com/BoozeLee](https://github.com/BoozeLee)

Every number below came out of a command you can run. The command is next to the number.

---

## harness — an AI engineering pipeline, measured against the agent it replaces

`scan` → `task` → `verify` → `pr`. A policy gate blocks protected-path writes and secret
reads before the edit lands, evidence is bound to each claim, and a PR will not open unless
the verdict is PASS — a skipped review counts as not passed.

```
pip install harness-agent        # hatchling wheel; 12 subcommands
pytest                           # -> 88 passed
harness eval run --agent codex   # raw agent vs the same agent under the harness
```

The evaluation is the part worth arguing about. 6 tasks, each run twice — once raw, once
harnessed — 13 runs, graded by a hidden acceptance suite the agent never sees:

- **11 / 13 graded PASS.** The only failure was one task, on both variants, on a genuine
  edge case in the agent's own output.
- Scope violations: **raw 3, harnessed 4.** The harness did not improve that number; the
  contract was amended after the runner flagged them. It is in the report because that is
  what the run produced.
- First-pass gates read FAIL on every harnessed run — the independent-review pass hit the
  provider session limit. Recorded, not skipped.

- 88 tests passing · 6,646 non-blank tracked lines (Python 4,378) · AGPL-3.0
- `harness scan --fail-under 70` exits 1 below the readiness floor
- Guard runs as a `PreToolUse` hook: a blocked write exits 2 and logs to `.ai-engineering/audit.log`
- [github.com/BoozeLee/harness](https://github.com/BoozeLee/harness)

## elohim — a gate for numerical claims

Six instruments measure hard mathematics, pin every result they claim, and refuse to pass if
anything moved — including the instrument itself.

```
git clone https://github.com/BoozeLee/elohim && cd elohim
python3 tests/test_all.py       # -> ALL_SKILLS_PASS
```

Then break something on purpose. The same command reports `verdict FAIL` with a `PIN DRIFT`
line naming the file whose checksum changed. A verification tool that cannot fail proves
nothing, so the tamper half is part of the gate itself:

- **6 / 6 injected-tamper cases caught**, each emitting `verdict FAIL` + `PIN DRIFT`
- Claim binding: 72 facts, 52 pinned values, 17 declared exemptions, **0 unclassified**
- 7 shipped skills · 19,831 non-blank tracked lines (Python 19,615) · MIT · CI + CodeQL green
- [github.com/BoozeLee/elohim](https://github.com/BoozeLee/elohim)

## terminal221b — a coding CLI bounded to a workspace, with a Rust TUI

An installable local-first CLI in TypeScript with a `ratatui` terminal UI, plus an Expo chat
client. Context is bounded by path rather than by a token budget, untrusted command output is
redacted before it reaches a stored transcript, and every patch passes a reviewed envelope.

```
npm ci && npm test               # -> 385 passed
cargo test -p terminal221b-tui   # -> 60 passed
```

- **445 tests total** (385 TypeScript + 60 Rust) · 55 commits · 16,210 non-blank tracked lines
- Test modules include `path-guard`, `boundary-drift`, `scope` and `security` — the
  containment properties, not only the happy paths
- AGPL-3.0 · [github.com/BoozeLee/terminal221b](https://github.com/BoozeLee/terminal221b)

## repotruth — CI that reads the repository, not just the diff

Indexes a repository into a knowledge graph, then exposes it three ways: an MCP server an
agent can query, a CLI, and a fleet service. It also receives webhooks, and it treats an
unverified push as an attack surface rather than as a fact:

```
npm ci && npm test               # -> 147 passed, 32 suites
node dist/src/bin.js audit .. --format json
```

- A correctly signed push is accepted. A **replayed** delivery answers `200` and does not
  re-run the scan. An **unsigned** push is rejected with `400` and nothing is queued. A
  **tampered body carrying an otherwise-valid signature** is rejected.
- `audit` emits `schemaVersion 1.0.0` and reports `truncated: false` rather than silently
  truncating when input exceeds its declared limits
- 5,974 non-blank tracked lines · AGPL-3.0
  · [github.com/Bakery-street-project/galacticfederation](https://github.com/Bakery-street-project/galacticfederation)

---

## Also built

- **mcp-regression-lab** — a GitHub Action that diffs an MCP server's tool contract across
  releases, because model upgrades rename and narrow tools without announcing it. 29 tests
  passing. [public](https://github.com/BoozeLee/mcp-regression-lab)
- **mycroft** — fixed-scope AI diagnostics that end in a written Minimum Viable Action.
  [public](https://github.com/BoozeLee/mycroft)
- Private, available to show on request: **capo** (349 tests across five packages),
  **superbrain** (298 passing tests), **beehive-studio** (54,550 non-blank tracked lines).

## How I work

Give an agent a task and it will report success whether or not it succeeded. The interesting
work is the part where you check. So I have built the checks I wanted to exist: instruments
that re-derive their own numbers, gates tested by being broken on purpose, harnesses measured
against the thing they are meant to replace — including when the measurement is unflattering.
That is the work I want to be paid for.

## What I don't claim

- **No degree, no certifications.** Self-taught.
- **No prior employment.** This is my first job. I have never been paid to write software and
  I do not describe myself as having been.
- **`Bakery-street-project` is a personal project of mine, not a company.** No customers, no
  revenue, no deployments. I do not call myself a founder of it.
- **No adoption story.** All seven of my public repositories have 0 stars, 0 forks and 0
  watchers. I have no users and no usage numbers.
- **Docker, Kubernetes and Go appear nowhere in my code.** I have not shipped a container or a
  cluster, and Go is listed here only so you know to discount it if a job ad asks for it.
- Everything above the line is verifiable by cloning the repository and running the command
  shown next to it.

---

![Profile views](https://komarev.com/ghpvc/?username=BoozeLee&style=flat-square&color=blue)