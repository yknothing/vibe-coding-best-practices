# Implementation Best Practices

*Effective code generation and refinement strategies*

[English](../../en/playbooks/implementation.md) | [中文](../../zh/playbooks/implementation.md)

## Overview

The implementation phase is where Vibe Coding delivers its most direct value. Through human-machine collaboration, code generation speed can be significantly improved while maintaining code quality and consistency. This guide introduces how to fully leverage AI assistance to accelerate the code implementation process while ensuring quality.

## Core Principles

The following Vibe Coding core principles should be followed during the implementation phase:

- **Memory & Navigation**: Utilize project memory to provide accurate context
- **Controlled Integrity of Change Units**: Ensure the consistency of code changes
- **Fidelity & Amplification of Value Stream**: Use AI as an amplifier for value realization
- **Closed-Loop Autonomy of Quality Calibration Circuits**: Establish immediate feedback and correction mechanisms

## Practical Steps

### 1. Context Preparation and Task Decomposition

**Goal**: Provide complete context for AI and decompose implementation tasks

**Best Practices**:
- Clearly define the scope and objectives of the current task
- Provide relevant code structure, interface definitions, and dependencies
- Break large implementation tasks into manageable subtasks
- Establish dependencies and priorities between tasks

**Anti-patterns**:
- Providing incomplete or irrelevant context
- Requesting overly complex implementations at once
- Lack of clear acceptance criteria

**Example Prompt**:
```
I need to implement [Function X]. The relevant context is as follows:
- Tech stack: [specific tech stack]
- Function objective: [specific description]
- Related interfaces: [interface definitions]
- Main dependencies: [related components/libraries]

Please help me:
1. Break down the implementation into logical steps
2. Provide implementation suggestions for each step
3. Point out technical aspects that require special attention
```

### 2. Iterative Code Generation and Optimization

**Goal**: Generate high-quality code through multiple iterations

**Best Practices**:
- First generate core functionality, then gradually refine and optimize
- Focus on one aspect of improvement in each iteration
- Provide specific feedback to guide the next iteration
- Maintain consistency in code style and structure

**Anti-patterns**:
- Accepting generated code without iterative improvement
- Providing vague feedback without specific guidance
- Ignoring code readability and maintainability

**Example Prompt**:
```
After reviewing the generated code:
"The [X part] of this code needs optimization, please:
1. Improve error handling logic
2. Enhance performance (especially for [specific scenario])
3. Ensure compliance with the project's naming conventions
4. Add necessary unit test coverage"
```

### 3. Code Quality Assurance and Review

**Goal**: Ensure generated code meets quality standards and design intent

**Best Practices**:
- Use AI assistance for code self-review
- Apply static analysis and automated testing to verify code quality
- Focus on edge cases and exception handling
- Ensure completeness of code comments and documentation

**Anti-patterns**:
- Skipping quality checks before integrating code
- Ignoring non-functional requirements like performance and security
- Lack of critical thinking about AI-generated code

**Example Prompt**:
```
For the generated [Module X] code:
1. Please check for potential security vulnerabilities
2. Evaluate if there's room for performance optimization
3. Verify if all boundary conditions are properly handled
4. Confirm if the code aligns with our design intentions
```

### 4. Knowledge Capture and Experience Reuse

**Goal**: Capture implementation experience as reusable patterns and knowledge

**Best Practices**:
- Record key decisions and techniques from the implementation process
- Distill common patterns and solutions into templates
- Update the project's "living documentation" system
- Use AI IDE's memory or rules system to store experience

**Anti-patterns**:
- Repeatedly solving the same problems without capturing experience
- Implementation knowledge existing only with individuals rather than shared with the team
- Lack of abstraction and distillation of implementation patterns

**Example Activities**:
- Regularly organize common code patterns and add them to the project template library
- Establish a Technical Decision Records (TDR) system
- Update the project's best practices guide

## Success Indicators

- Increased code implementation speed
- Code quality metrics (such as complexity, coverage) meeting standards
- Reduced defect density
- Gradually shortened implementation time for similar features

## IDE Implementation References

- [Cursor Implementation Guide](../ai-ide/cursor/overview.md)
- [Windsurf Implementation Guide](../ai-ide/windsurf/overview.md)

---

## Further Reading

- [Design Best Practices](./design.md)
- [Maintenance Best Practices](./maintenance.md)
- [Memory & Navigation Principle](../principles/golden-rules.md#5-memory--navigation-in-state-space)
