# Execution Engine

## Purpose

Execute validated trading decisions through provider adapters.

---

## Responsibilities

- Build transactions
- Sign transactions
- Submit transactions
- Retry failed executions
- Confirm transactions

---

## Inputs

Validated Trading Decision

---

## Outputs

Execution Result

---

## Produced Events

ExecutionStarted

ExecutionCompleted

---

## Rules

Never generate trading decisions.

Never modify strategy logic.

Execute only approved decisions.