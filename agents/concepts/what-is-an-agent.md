# What Is An AI Agent

## Core Idea

An AI agent is a system that can reason, take actions, observe results, and continue making decisions until a task is completed.

## Agent Loop

```text
Thought → Action → Observation
```

## Example

```text
Thought:
Need weather information

Action:
Call weather API

Observation:
Temperature is 18°C

Thought:
Now generate final answer
```

## Why LLMs Alone Are Limited

LLMs alone cannot:

- access real-time data
- persist memory reliably
- execute tools
- manage workflows
- coordinate multi-step tasks

## Why Tools Matter

Tools allow agents to interact with external systems such as:

- APIs
- databases
- search systems
- file systems
- code execution

## Agent vs Workflow

Workflows are predefined execution paths.

Agents dynamically decide what actions to take.

## Failure Modes

- infinite loops
- wrong tool selection
- hallucinated actions
- memory failures
- bad planning

## Observations

- Agents are much more than chatbots.
- Tool usage changes how LLM systems behave.
- Reasoning loops create flexibility.

## Open Questions

- How do agents decide which tool to use?
- How do frameworks prevent infinite loops?
- How does memory persist between actions?
