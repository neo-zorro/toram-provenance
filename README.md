# TORAM public product direction

**Financial-market intelligent infrastructure for systematic trading — from one instrument in a user's hands to professional and institutional workflows.**

TORAM is being developed around a simple idea:

> **Define the strategy. Keep every decision visible. Use the same logic from replay to the live market.**

A user should be able to begin with one supported instrument, define entry / wait / hold / exit / risk conditions as explicit gates, replay recorded market history, and run the same strategy definition against the live market in paper mode.

Where supported and explicitly enabled, the same gated path can later become eligible for controlled broker execution.

## The workspace

TORAM is designed as an inspectable trading workspace rather than a black-box signal generator.

The core experience is:

1. choose a supported instrument;
2. define the strategy and its gates;
3. replay recorded market state;
4. inspect why the strategy waited, entered, held or exited;
5. run the same definition in live paper; and
6. keep real execution behind separate user, risk, broker and account permissions.

The value is continuity and inspectability: the strategy should keep the same meaning while the market-state source moves from replay to live.

## Junction gates

A junction is where current market state meets strategy, position, risk and execution rules.

```text
market state
  -> strategy gates
  -> position state
  -> risk permission
  -> paper / approved execution
  -> result
```

The user should be able to see which gate passed, failed or changed before an action occurs.

## Replay, live paper and live execution

### Replay

Use recorded market history to inspect the decision path and state transitions.

### Live paper

Run the same strategy definition against the current market without sending real orders.

### Live execution

Where supported and explicitly enabled, an eligible strategy can produce broker execution intents through the same controlled path.

### Review

Return to the timeline afterward and understand what the strategy saw, which gate changed and why the state moved.

## Who TORAM is for

The same core model is intended to become deeper as the user becomes more sophisticated.

### Self-directed users

One instrument, one strategy, replay, live paper and a visible decision timeline.

### Pro traders and pro desks

Richer strategy definitions, multiple strategy versions, stronger diagnostics and controlled execution workflows.

### Quant desks

Reusable state definitions, multiple instruments, replay, diagnostics and team-level strategy controls.

### Institutions, funds and brokers

Private deployment, entitlements, broker reconciliation, auditability and stronger production-assurance workflows.

The goal is not to force every user into institutional complexity. The same underlying concepts should remain understandable at every level.

## Product principle

> **Every action should have a visible reason.**

TORAM keeps strategy logic, position state, risk permission and execution authority as distinct parts of the operating path.

A useful system should show more than the final trade or P&L. It should make it possible to understand what state the strategy was in and why that state changed.

## Vision

The long-term direction is:

> **One operating environment for trading intelligence.**

Start with a single user's strategy. Extend the same principles across instruments, brokers, teams, asset classes and institutional controls without losing inspectability.

The common workflow remains:

> **Define → Replay → Live Paper → Controlled Execution → Review**

## Public disclosure boundary

The public page intentionally avoids proprietary strategy mathematics, private runtime implementation details, credentials, investor materials, internal engineering evidence, customer information and unsupported return claims.

Product descriptions are directional and may change. Nothing on the page is investment advice, a recommendation, a performance claim, a guarantee of returns or a claim of regulatory approval.
