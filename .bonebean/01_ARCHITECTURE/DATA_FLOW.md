# Data Flow

## Purpose

This document defines how data moves throughout Bone Bean AI.

The objective is to ensure a predictable, traceable, and deterministic processing pipeline.

---

# High-Level Flow

```
Market Provider
        │
        ▼
Provider Adapter
        │
        ▼
Market Engine
        │
        ▼
Feature Engine
        │
        ▼
Probability Engine
        │
        ▼
Decision Engine
        │
        ▼
Risk Engine
        │
        ▼
Execution Engine
        │
        ▼
Portfolio Engine
        │
        ▼
Reporting
```

---

# Stage 1 — Market Data

Input

- DEX
- RPC
- Meteora
- Helius
- DexScreener
- GMGN

Output

Normalized market data.

---

# Stage 2 — Feature Extraction

Generate:

- Volatility
- Liquidity
- Holders
- Fees
- APR
- Market Cap
- Volume

---

# Stage 3 — Probability

Calculate:

- Expected Return
- Confidence Score
- Risk Score

---

# Stage 4 — Decision

Evaluate strategy rules.

Possible outputs:

- BUY
- SELL
- HOLD
- REBALANCE
- HARVEST

---

# Stage 5 — Risk Validation

Validate:

- Exposure
- Drawdown
- Allocation
- Limits

---

# Stage 6 — Execution

Execute transactions through provider adapters.

---

# Stage 7 — Portfolio Update

Update:

- Positions
- PnL
- Treasury
- Allocation

---

# Stage 8 — Reporting

Generate:

- Dashboard
- Metrics
- Analytics
- History

---

# Data Principles

Every transformation must be deterministic.

Every output must be reproducible.

Every stage must produce structured logs.

No stage may mutate upstream data.

---

# Version

Current Version: 1.0
Status: Draft