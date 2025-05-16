# Requirements Analysis Best Practices

*Techniques for clear intent definition and requirements gathering with AI assistance*

[English](../../en/playbooks/requirements.md) | [中文](../../zh/playbooks/requirements.md)

## Overview

Requirements analysis is the first step in software development and one of the most critical phases. In the Vibe Coding paradigm, human-AI collaboration can significantly improve the efficiency and quality of requirements analysis, provided the right practices are followed.

This guide introduces how to conduct effective requirements analysis in an AI-assisted environment, ensuring that human intentions can be accurately mapped to the development process.

## Core Principles

The following Vibe Coding core principles should be followed during the requirements analysis phase:

- **Isomorphic Mapping of Intent**: Ensuring that high-level human intentions can be accurately understood by AI
- **Order from Entropy Reduction & Consensus Reality**: Reducing ambiguity in requirements through structured methods
- **Memory & Navigation**: Establishing a persistent requirements memory system

## Practical Steps

### 1. Intent Initialization

**Goal**: Create clear high-level intent statements

**Best Practices**:
- Use structured templates to describe project goals and scope
- Clearly distinguish between functional and non-functional requirements
- Establish an initial list of constraints
- Use AI to help refine and clarify ambiguous concepts

**Anti-patterns**:
- Incomplete or overly vague requirement descriptions
- Mixing multiple unrelated intentions
- Lack of clear priorities and importance indicators

**Example Prompt**:
```
I need to develop a [product type] that solves [core problem].
Core functionalities include:
1. [Function 1]
2. [Function 2]
...

Non-functional requirements:
- Performance: [specific requirements]
- Security: [specific requirements]
- Scalability: [specific requirements]

Technical constraints:
- [Constraint 1]
- [Constraint 2]
...

Please help me analyze the completeness and consistency of these requirements, pointing out potential conflicts or ambiguities.
```

### 2. Requirement Refinement and Decomposition

**Goal**: Break down high-level requirements into well-defined tasks that AI can process

**Best Practices**:
- Use user stories or scenario descriptions
- Apply structured formats (such as the INVEST criteria)
- Leverage AI to ask clarifying questions and identify boundary conditions
- Create requirements traceability matrix

**Anti-patterns**:
- Over-decomposition leading to loss of global perspective
- Lack of correlation and consistency between requirements
- Ignoring edge cases and exception flows

**Example Prompt**:
```
For [Function X], please help me:
1. Break it down into independent user stories
2. Define acceptance criteria for each story
3. Identify potential edge cases and exception flows
4. Suggest key questions I might have overlooked
```

### 3. Requirement Validation and Consensus Building

**Goal**: Ensure all stakeholders have a consistent understanding of requirements

**Best Practices**:
- Create requirement prototypes or visual representations
- Use AI to generate requirement interpretations from different perspectives
- Establish a process for evaluating requirement changes
- Use living documents to record decisions and consensus

**Anti-patterns**:
- Skipping validation and proceeding directly to implementation
- Frequent changes after requirements consensus
- Lack of mechanisms to track requirement changes

**Example Prompt**:
```
Based on our discussion of [Function X]:
1. Please generate a simple interface prototype description
2. Explain this feature from the perspective of users, developers, and testers
3. List the technical challenges in implementing this feature
4. Suggest possible alternatives and trade-offs
```

### 4. Requirement Memory Persistence

**Goal**: Establish a continuously accessible requirements memory system

**Best Practices**:
- Create structured requirement documents
- Use AI IDE's memory or rules system to store key decisions
- Establish bidirectional traceability between requirements and code
- Regularly review and update requirement status

**Anti-patterns**:
- Relying on temporary conversations rather than persistent documentation
- Lack of requirement change history
- Requirements scattered across multiple systems

## Success Indicators

- Requirement change frequency within reasonable range
- High consistency between implementation and requirements
- Low rework rate during development
- Team members have consistent understanding of project goals

## IDE Implementation References

- [Cursor Implementation Guide](../ai-ide/cursor/overview.md)
- [Windsurf Implementation Guide](../ai-ide/windsurf/overview.md)

---

## Further Reading

- [Design Best Practices](./design.md)
- [Isomorphic Mapping of Intent Principle](../principles/golden-rules.md#2-isomorphic-mapping-of-intent)
