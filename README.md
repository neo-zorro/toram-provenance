# TORAM

**Governed financial runtime for causal state, controlled action and replayable evidence**

TORAM is a working financial runtime built first around NIFTY futures and options. The system connects durable market state, temporal intelligence, deterministic authority, controlled broker execution and replayable evidence in one operating chain.

The product direction is to make those runtime contracts reusable across supported instruments and broker-connected financial workflows without making any single model, feed or broker the product boundary.

## What exists today

The private operating stack already covers the core runtime primitives:

- durable live market capture and historical replay;
- one causal decision path across live and replay;
- deterministic capital, session, freshness and risk authority;
- fail-closed transport and execution boundaries;
- controlled broker execution and order/position reconciliation;
- charge-aware execution reporting and post-trade evidence.

Controlled full-session tests have reproduced live decision timing and state-machine behavior from recorded market history, and broker-linked LIVE execution has been exercised through a separate signed execution service.

## Product thesis

TORAM organizes financial action as:

`Data → Intelligence → Authority → Action → Evidence`

Models, feeds and brokers can change. The runtime contract keeps time, permission, action and evidence coherent.

**Generative where useful. Deterministic where authority matters.**

## Product direction

The runtime is being generalized through explicit capabilities and adapters:

1. **Reference runtime** — continue hardening the existing NIFTY derivatives implementation.
2. **Reusable financial runtime** — extract instrument capabilities, broker adapters, permissions, observability and validation.
3. **Connected workflows** — extend across supported instruments, professional workflows, private deployments and API/runtime surfaces.

An instrument is not considered supported until its data, execution, risk and evidence contracts are production-ready.

## Public disclosure boundary

Safe to discuss publicly:

- the working financial-runtime thesis;
- high-level data / intelligence / authority / action / evidence architecture;
- the NIFTY futures/options proving ground;
- live/replay discipline and fail-closed controls;
- controlled broker execution and reconciliation at a high level;
- multi-instrument product direction.

Not published here:

- proprietary strategy formulas, thresholds, weights or calibration;
- strategy-specific feature definitions or model artifacts;
- raw decision-audit datasets or private broker records;
- credentials, infrastructure addresses, internal repositories or source code;
- unsupported, annualized or extrapolated performance claims;
- private commercial or financing materials.

## Technology

This public site is deliberately static and lightweight:

- semantic HTML;
- Tailwind CSS v4, compiled at deploy time;
- GitHub Pages;
- GitHub Actions deployment;
- no client-side framework or analytics dependency.

Deployment is handled by `.github/workflows/deploy-pages.yml`.

For first-time GitHub Pages activation:

**Settings → Pages → Build and deployment → Source → GitHub Actions**

Then run or re-run the **Deploy TORAM Provenance** workflow.

## Public purpose

This repository is a public product and technology overview. It is informational and is not investment advice, a brokerage service or a guarantee of financial performance.
