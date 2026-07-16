# Event Flow

## Purpose

This document defines how events propagate throughout Bone Bean AI.

Events provide loose coupling between independent modules while maintaining deterministic execution.

---

# Event Pipeline

```
Market Updated
        │
        ▼
Features Generated
        │
        ▼
Probability Calculated
        │
        ▼
Decision Generated
        │
        ▼
Risk Validated
        │
        ▼
Execution Started
        │
        ▼
Execution Completed
        │
        ▼
Portfolio Updated
        │
        ▼
Report Generated
```

---

# Core Events

## MarketUpdated

Published when new market data is available.

---

## FeaturesGenerated

Published after feature extraction.

---

## ProbabilityCalculated

Published after probability analysis.

---

## DecisionGenerated

Published after deterministic decision making.

---

## RiskValidated

Published after successful risk evaluation.

---

## ExecutionStarted

Published before submitting a transaction.

---

## ExecutionCompleted

Published after execution completes.

---

## PortfolioUpdated

Published after balances and positions change.

---

## ReportGenerated

Published when analytics are refreshed.

---

# Event Rules

Events must be immutable.

Events must contain timestamps.

Events must contain correlation IDs.

Events must be versioned.

Events must never contain secrets.

---

# Benefits

Loose coupling.

Independent services.

Plugin compatibility.

Scalability.

Auditability.

Observability.

---

# Version

Current Version: 1.0
Status: Draft