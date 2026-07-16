# Engine

The Engine domain defines every deterministic processing engine used by Bone Bean AI.

These engines transform raw market data into deterministic trading decisions. Engine behavior must always be predictable, testable, and independent from LLM reasoning.

---

# Responsibilities

- Process market data
- Generate deterministic signals
- Execute calculation pipelines
- Produce trading decisions
- Manage execution workflow
- Remain deterministic under identical inputs

---

# Reading Order

1. MARKET_ENGINE.md
2. FEATURE_ENGINE.md
3. PROBABILITY_ENGINE.md
4. DECISION_ENGINE.md
5. ENTRY_ENGINE.md
6. EXIT_ENGINE.md
7. EXECUTION_ENGINE.md
8. PORTFOLIO_ENGINE.md
9. RISK_ENGINE.md
10. SIMULATION_ENGINE.md

---

# Document Index

| Document | Status | Description |
|----------|--------|-------------|
| MARKET_ENGINE.md | ⏳ Planned | Market data aggregation |
| FEATURE_ENGINE.md | ⏳ Planned | Feature extraction |
| PROBABILITY_ENGINE.md | ⏳ Planned | Probability calculations |
| DECISION_ENGINE.md | ⏳ Planned | Deterministic decision logic |
| ENTRY_ENGINE.md | ⏳ Planned | Entry validation |
| EXIT_ENGINE.md | ⏳ Planned | Exit validation |
| EXECUTION_ENGINE.md | ⏳ Planned | Order execution |
| PORTFOLIO_ENGINE.md | ⏳ Planned | Portfolio management |
| RISK_ENGINE.md | ⏳ Planned | Risk evaluation |
| SIMULATION_ENGINE.md | ⏳ Planned | Backtesting & paper trading |

---

# Engineering Rules

- Engines must be deterministic.
- Engines must not invoke LLMs directly.
- Every engine requires a specification before implementation.
- Every public interface must be documented.
- Every engine must include unit and integration tests.
- Engine communication should occur through defined interfaces or events.

---

# Deliverables

Each engine specification should include:

- Purpose
- Responsibilities
- Inputs
- Outputs
- Processing Flow
- Public Interfaces
- Events
- Configuration
- Error Handling
- Performance Requirements
- Testing Strategy

---

# Current Status

**Version**

0.1.0

**Specification Progress**

0 / 10 Complete

**Implementation Progress**

0 / 10 Complete

**Testing Progress**

0 / 10 Complete

---

# Next Milestone

Complete MARKET_ENGINE.md