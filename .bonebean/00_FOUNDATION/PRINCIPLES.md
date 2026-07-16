# Engineering Principles

## Purpose

This document defines the engineering principles that guide every architectural and implementation decision within Bone Bean AI.

These principles apply to all contributors, AI assistants, and future engineering teams.

---

# Principle 1

Deterministic Execution

Trading decisions must always produce identical results when given identical inputs.

---

# Principle 2

AI Assists, Engine Decides

Artificial Intelligence may generate ideas, explanations, or optimizations.

Only deterministic engines are allowed to execute trading logic.

---

# Principle 3

Architecture Before Implementation

Major features require an approved architecture and specification before implementation begins.

---

# Principle 4

Security by Default

Security is part of every feature rather than an afterthought.

---

# Principle 5

Plugin First

New capabilities should be added through extension points whenever practical instead of modifying the core system.

---

# Principle 6

API First

All platform capabilities should be exposed through stable, versioned APIs.

---

# Principle 7

Documentation is Part of the Product

Documentation evolves together with implementation.

Outdated documentation is treated as a defect.

---

# Principle 8

Observability by Default

Every important process should produce logs, metrics, and traces suitable for monitoring and debugging.

---

# Principle 9

Version Everything

Strategies, APIs, specifications, configurations, and plugins must be versioned to ensure compatibility and traceability.

---

# Principle 10

Keep the Core Small

The core platform should remain focused, while additional functionality is implemented through plugins or independent modules whenever practical.

---

# Decision Rule

When multiple solutions are available, choose the one that is:

1. Simpler
2. Easier to maintain
3. Easier to test
4. Easier to extend
5. Easier to understand

---

# Non-Negotiable Rules

- Never allow AI to execute trades directly.
- Never expose user secrets or private keys.
- Never bypass deterministic engine validation.
- Never merge undocumented architecture changes.
- Never sacrifice security for convenience.