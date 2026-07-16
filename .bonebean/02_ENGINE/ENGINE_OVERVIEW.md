# Engine Overview

## Purpose

The Engine layer is the deterministic core of Bone Bean AI.

It transforms market data into validated trading actions through a sequence of independent processing engines.

Unlike AI components, every engine produces deterministic and reproducible outputs.

---

# Objectives

- Deterministic execution
- Modular processing
- High performance
- Testability
- Extensibility
- Observability

---

# Engine Pipeline

```
Market Engine
        │
        ▼
Feature Engine
        │
        ▼
Scoring Engine
        │
        ▼
Probability Engine
        │
        ▼
Decision Engine
        │
        ▼
Entry / Exit Engine
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
Harvest Engine
        │
        ▼
Rebalance Engine
        │
        ▼
Report Engine
```

---

# Engine Responsibilities

| Engine | Responsibility |
|---------|----------------|
| Market | Collect market data |
| Feature | Extract trading features |
| Scoring | Calculate weighted scores |
| Probability | Estimate probabilities |
| Decision | Produce deterministic decisions |
| Entry | Validate entry opportunities |
| Exit | Validate exit conditions |
| Risk | Validate trading risks |
| Execution | Execute transactions |
| Portfolio | Maintain positions |
| Harvest | Collect rewards |
| Rebalance | Optimize allocation |
| Report | Generate analytics |
| Watchlist | Track monitored assets |

---

# Design Principles

Every engine must:

- Have one responsibility.
- Be independently testable.
- Be deterministic.
- Expose documented interfaces.
- Emit structured events.
- Never invoke LLMs.

---

# Engine Lifecycle

Input

↓

Processing

↓

Validation

↓

Output

↓

Event

↓

Logging

↓

Metrics