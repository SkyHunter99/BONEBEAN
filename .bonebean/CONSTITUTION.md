# BONE BEAN AI CONSTITUTION

Version: 1.0

---

# Vision

Bone Bean AI is an AI-powered Liquidity Provider Operating System.

It is NOT an LP Bot.

It is NOT a Trading Bot.

It is an extensible operating system that allows users to build, execute, optimize, automate, and monetize Liquidity Provider strategies.

---

# Core Philosophy

The platform must remain modular.

Every module has a single responsibility.

Every module must be replaceable.

Every module must be testable.

Every module must be independent.

Never sacrifice architecture for speed.

Always prioritize maintainability.

---

# Architecture Principles

The architecture follows strict separation of responsibility.

Apps

↓

Strategy

↓

Runtime

↓

Engine

↓

Execution

↓

Providers

AI is always separated from trading execution.

---

# Golden Rule #1

ENGINES MUST NEVER USE LLM.

Never call:

OpenAI

Claude

Gemini

OpenRouter

Ollama

inside any Engine.

Engines must always be deterministic.

Given the same input,

the output must always be identical.

---

# Golden Rule #2

AGENTS ALWAYS USE LLM.

Agents are responsible for reasoning only.

Agents never execute trades.

Agents never calculate indicators.

Agents never decide execution.

Agents produce knowledge.

Engines execute knowledge.

---

# Golden Rule #3

STRATEGY IS DATA.

Strategies are configuration.

Strategies are NOT code.

Strategies must be serializable.

Strategies must be exportable.

Strategies must be importable.

Strategies must be versioned.

Strategies must be portable.

Preferred format:

JSON

---

# Golden Rule #4

RUNTIME NEVER DEPENDS ON AI.

Once a strategy is compiled,

Runtime executes it without AI.

Removing AI must never stop Runtime.

---

# Golden Rule #5

EVERY FEATURE MUST BE PLUGGABLE.

Indicators

Providers

Strategies

Notifications

Exchanges

must all support plugins.

---

# Golden Rule #6

ALL PROVIDERS MUST USE ADAPTERS.

Never call APIs directly inside Engines.

Every provider must expose interfaces.

Example

MarketProvider

↓

GMGN

DexScreener

Birdeye

Meteora

LPAgent

Helius

---

# Golden Rule #7

USER OWNS THEIR AI.

Bone Bean AI never forces users to use one AI provider.

Supported providers

OpenAI

Claude

Gemini

OpenRouter

Ollama

Future providers

should require zero architecture changes.

---

# Golden Rule #8

MARKET DATA IS PLATFORM RESPONSIBILITY.

Bone Bean AI manages:

GMGN

LPAgent

Meteora

Helius

Birdeye

DexScreener

RugCheck

BubbleMaps

Users should never need to configure these providers.

---

# Golden Rule #9

BUSINESS MODEL

Revenue comes from Strategy Marketplace.

Creators publish strategies.

Users purchase strategies.

Bone Bean receives marketplace commission.

No AI subscription business model.

---

# Golden Rule #10

EVERY DECISION MUST BE EXPLAINABLE.

Every Entry

Every Exit

Every Harvest

Every Rebalance

must have explanation logs.

The platform should always answer

"Why did this happen?"

---

# Golden Rule #11

NO MAGIC NUMBERS.

Everything configurable.

Thresholds

Indicators

Risk

Weights

Timing

Fees

Market Filters

All configurable.

---

# Golden Rule #12

NO HARD CODED STRATEGIES.

Never create

Panda Strategy

Vladimir Strategy

etc.

Strategy Builder must support unlimited strategies.

---

# Golden Rule #13

BACKTEST FIRST.

Every strategy should support

Backtesting

↓

Paper Trading

↓

Live Trading

Never encourage direct Live Trading.

---

# Golden Rule #14

MULTI TENANT FIRST.

Every feature must assume

multiple organizations

multiple users

multiple wallets

multiple strategies.

Never build for a single user.

---

# Golden Rule #15

SECURITY FIRST.

Never store wallet private keys.

Never expose API Keys.

Always encrypt secrets.

Always audit executions.

Always log changes.

---

# Golden Rule #16

CODE QUALITY

Use:

Clean Architecture

SOLID

DRY

KISS

Composition over Inheritance

Explicit Interfaces

Dependency Injection

Every public module

must have tests.

---

# Golden Rule #17

PROJECT STRUCTURE

Apps

Core

Providers

Engines

Agents

Strategy

Marketplace

Lab

Insights

Portfolio

Automation

AI

Plugins

Monitoring

Notification

Security

Database

Storage

Docs

No module may bypass the architecture.

---

# Golden Rule #18

AI RESPONSIBILITY

AI may:

Explain

Reason

Optimize

Import

Generate

Summarize

Validate

AI may NOT:

Execute trades

Open LP

Close LP

Harvest

Transfer assets

Sign transactions

---

# Golden Rule #19

PERFORMANCE

Always minimize:

API Calls

Database Queries

Memory Usage

CPU Usage

Latency

Support:

Cache

Queue

Parallel Processing

Streaming

Worker Architecture

---

# Golden Rule #20

LONG TERM THINKING

Every design decision should still make sense

five years from today.

Avoid temporary solutions.

Avoid shortcuts.

Avoid duplicated logic.

Design for growth.

---

# Development Workflow

Requirement

↓

Architecture

↓

Domain Design

↓

Implementation

↓

Unit Test

↓

Integration Test

↓

Backtest

↓

Paper Trade

↓

Production

---

# Final Principle

Bone Bean AI is not a trading bot.

Bone Bean AI is an Operating System for Liquidity Providers.

Every line of code should move the platform closer to that vision.