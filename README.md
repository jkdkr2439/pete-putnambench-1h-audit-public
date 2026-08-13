# Pete PutnamBench One-Hour Audit

This repository preserves a disclosure-limited, trace-based audit of a one-hour natural-language run over the complete 673-item informal PutnamBench corpus snapshot.

## Recorded setup

- Researcher and framework designer: Kevin T.N, epistemology researcher
- Tested deployment label: GPT-5.6 Sol Light in Codex Desktop, as operator-designated for the run
- Model class: general-purpose coding/agent model, not represented here as mathematics-specialized
- Framework: Pete / Math Fieldmap, a human-designed epistemic scaffold
- Run window: 2026-08-13 20:31:41 UTC to 21:31:41 UTC
- Corpus snapshot: upstream commit `dfb0a47a1c1ec3a10f2a9acfdf41a2043920f33c`

The experiment separates immutable natural-language proof candidates, post-lock answer agreement, manual self-audit, failures, unresolved gaps, contamination, and formal proof-assistant verification. Answer agreement is not proof verification. The formal score is `0/673` because no candidate was accepted by a proof kernel.

## Contents

- `paper/`: LaTeX source
- `output/pdf/`: rendered paper
- `evidence/RUN_LOG.jsonl`: append-only hash-chained event log
- `evidence/PROOF_LOCKS.jsonl`: immutable proof hashes
- `evidence/OUTCOMES.json`: one row for every corpus item
- `evidence/proofs/`: locked candidates and explicitly uncounted drafts
- `provenance/SHA256SUMS.txt`: artifact inventory

## Disclosure boundary

The repository does not contain the Fieldmap implementation, private maps, gates, rules, graph schemas, prompts, orchestration logic, or sealed reference solutions. The paper describes only the observable protocol needed to interpret the evidence.

## Build

Compile `paper/main.tex` twice with XeLaTeX. The committed PDF is the audited output.

