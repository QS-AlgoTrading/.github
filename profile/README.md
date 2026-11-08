# QS-AlgoTrading — QuantStand

**Pillar 2 of the Eterne Foundation: algorithmic trading.** QuantStand is a
family-office trading platform — macro intelligence, quantitative research, and
algorithmic execution across isolated engines, with real and paper capital never
conflated and every number carrying its provenance.

This organization operates under the **[Eterne Compass](https://github.com/eternecompass)**
— the group-wide operational governance doctrine for software development
(principles, session protocols, security baseline, engineering playbook). Start
at [`project-kickoff`](https://github.com/eternecompass/project-kickoff); the
org-local development protocol is
[`docs/DEVELOPMENT_WORKFLOW.md`](https://github.com/QS-AlgoTrading/docs/blob/main/DEVELOPMENT_WORKFLOW.md)
(**DEC-QNT-011** — branch-protected trunk, PR-only, serialized deploys).

**Lifecycle phase: 2 (Production)** — live real-money trading since 2026-06-17
(declaration: DEC-QNT-012). Org repo code: **`QNT`**.

---

## Repositories

| Repo | Role | Status |
|---|---|---|
| [`QuantStand-Ant`](https://github.com/QS-AlgoTrading/QuantStand-Ant) | Backend platform — engines, data plane, macro module, factory (private) | **Active · live** |
| [`quantstand-web`](https://github.com/QS-AlgoTrading/quantstand-web) | quantstand.com — the platform web app (private) | **Active · live** |
| [`docs`](https://github.com/QS-AlgoTrading/docs) | Tier-2 org documentation — architecture, decisions, session summaries | Active |
| [`cTrader-Algo-strategies`](https://github.com/QS-AlgoTrading/cTrader-Algo-strategies) | cTrader/FxPro strategy line (private) | Active-secondary |
| [`optionlab`](https://github.com/QS-AlgoTrading/optionlab) | Options strategy analysis on ORATS data — analysis-only, never trades (private; DEC-QNT-062) | Paused · not deployed |
| [`External-Connection`](https://github.com/QS-AlgoTrading/External-Connection) | Public signal layer | Public |
| `OpenClaw-Bot` · `Grid-Strategy-Learning` · `Medallion-thinking-Quant-Work` · `Regiem-Detection` | Early research holdings (private) | Museum / experimental |

---

## Governance quick facts

- `main` on the deploying code repos is **branch-protected**: PR required
  (admins included), required CI checks, up-to-date-before-merge, no
  force-pushes. Direct pushes are machine-rejected.
- Decision records: **`DEC-QNT-NNN`** in
  [`docs/decisions/`](https://github.com/QS-AlgoTrading/docs/tree/main/decisions)
  (existing `DEC-QS-*` ids are grandfathered), referencing up to the governing
  `ADR-CMP`/`ADR-EG`.
- Secrets never in git; templates ship blank. Trading credentials are
  least-privilege and never withdrawal-capable.
