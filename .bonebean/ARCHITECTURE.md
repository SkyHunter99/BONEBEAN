# Architecture

The architecture follows strict domain separation.

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

AI is never inside Engine.

Engine is always deterministic.

Agents are the only modules allowed to use LLM.

Runtime executes compiled strategies without AI.

Strategy is JSON.

Every strategy is portable.

Every strategy is versioned.

Every strategy is marketplace-ready.