# RunBook To Rule Them All

**In one line:** a place to write down *how I actually got something working* — so that
next time (me or an AI helper) I can follow the steps instead of figuring it all out
again from scratch.

> One node in a personal AI ecosystem — see the [ecosystem map](https://github.com/Nightmarejam).
> Human-directed, AI-assisted (see [PROVENANCE.md](PROVENANCE.md)). MIT licensed.

---

## The idea (one concept)

I have a goldfish memory for procedures — I solve something hard, then a month later I'm
re-deriving it from zero. A runbook fixes that: a **dated, followable, verifiable
recipe** for a repeatable task. External memory for procedures. The point isn't to
document for its own sake — it's so a task done once becomes a task anyone (including
future-me) can repeat without the original struggle.

## What lives here

| Path | Purpose |
|------|---------|
| `runbooks/entries/` | Dated runbook entries (`YYYY-MM-DD_<slug>.md`) |
| `runbooks/templates/` | Scaffolds (standard / sandbox / investigation) |
| `sandbox/examples/` | Runnable examples referenced by runbooks |
| `docs/architecture.md` | Design and conventions |

Each entry carries a `status`: `draft` → `verified` (someone actually followed it and it
worked). That status *is* the attestation — a runbook isn't trusted until it's been
replicated.

## Add one

```bash
./scripts/new_runbook.sh my-process-name   # writes a dated entry from the template
./scripts/validate.sh                      # check structure
```

Candidate runbooks are surfaced automatically from my conversation history by a scanner
in the (private) homelab pipeline — the corpus is mined for repeatable procedures worth
capturing here.

## Status & scope

Active, working ops knowledge — but scoped to *my* systems. Useful as reference and as a
pattern for building your own procedural memory, not a universal ops manual.
