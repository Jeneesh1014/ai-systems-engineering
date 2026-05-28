# AI System vs API Wrapper

## Problem

A single LLM API call is not enough for real-world AI applications because production systems require memory, workflows, routing, monitoring, retries, and tool integration.

## Why It Matters

Simple API wrappers work for demos but fail in production environments where systems must handle complex tasks, multi-step workflows, asynchronous execution, and long-term state.

## Simple API Architecture

```text
User → Prompt → LLM API → Response
```

## AI System Architecture

```text
User
 ↓
Orchestrator
 ↓
Memory + Tools + Routing
 ↓
LLM
 ↓
Validation
 ↓
State Update
 ↓
Response
```

## Core Concepts

- State
- Workflow
- Orchestration
- Routing
- Memory
- Async execution
- Event-driven systems

## Tradeoffs

### Simple API Wrappers

- easy to build
- low complexity
- limited scalability

### AI Systems

- scalable
- flexible
- production-ready
- harder debugging

## Observations

- Real AI systems are orchestration systems around LLMs.
- The LLM itself is only one component.
- State management seems extremely important.

## Open Questions

- How is state shared across distributed systems?
- How do agents coordinate memory?
- How do orchestration frameworks manage failures?
