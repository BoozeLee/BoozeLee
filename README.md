# Kiliaan Vanvoorden

I build the checks that decide whether an AI system is right — and the small, local-first tools that make that checkable by hand.

**Open to AI engineering and creative-tools roles.** Based in Riemst, Belgium · open to remote · employment or contract.

📧 [bakerstreetbandit@zohomail.eu](mailto:bakerstreetbandit@zohomail.eu)

## Public work

### [murmur](https://github.com/BoozeLee/murmur) — a one-button painting idea deck · Next.js + TypeScript

A web app for one painter who freezes in front of the easel. One press gives one idea: what to paint, the artistic problem inside it, where the light comes from, a palette, and a single line she can read from the easel. Keep it or refuse it — refused cards stop coming back.

No account, no notifications, no feed. The deck is the product. A daily push notification was built and then deliberately removed because nobody asked for it.

- **Corpus-first:** 53 hand-written cards answer instantly (~100 ms). A local 30B mixture-of-experts model writes new cards overnight while the machine is idle, so waiting on a model is never part of asking for an idea.
- **Bounded generation:** the on-demand writer produces a card through a JSON Schema it cannot escape (~40–65 s).
- **Local-first:** the core path has no cloud dependency, and the deck remembers refusals so it adapts to one person's taste instead of an engagement metric.

## How I work

Give an agent a task and it will report success whether or not it succeeded. The interesting work is the part where you check. So I build the checks I wanted to exist: instruments that re-derive their own numbers, gates that are tested by being broken on purpose, and evaluations that publish the unflattering result alongside the good one. That is the work I want to be paid for.

## Selected work — private, available to show on request

I keep most repositories private by choice. I can walk through any of these live:

- **elohim** — 103 facts with 122 checksum-pinned values, and six seeded tampering tests that must fail.
- **harness** — a contract-gated agent pipeline where a skipped review is not a pass.
- **terminal221b** — a coding CLI bounded by path, not by token budget.
- **repotruth** — CI that reads the repository, not just the diff; signed webhook verification.
- **cryptojukebox** — browser-local audio analysis that turns owned music into creative artifacts.
- **verification-spine** — stdlib-only Python that refuses to call a claim proven unless its evidence could actually have failed.

## Honest scope

No degree or certifications, and no prior employment — this would be my first role. `Bakery-street-project` and `Quattro-Commas` are my personal projects, not companies. Every number I quote was produced by a command I can re-run.
