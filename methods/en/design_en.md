# Design Best Practices

*Collaborative architecture and design approaches with AI*

[English](../../en/playbooks/design.md) | [中文](../../zh/playbooks/design.md)

## Overview

In the Vibe Coding paradigm, the design phase is a key moment for synergy between human creativity and AI capabilities. Good design not only meets functional requirements but also considers how to make the system more "AI-friendly" for smoother human-machine collaboration in subsequent development processes.

This guide introduces how to conduct efficient system design in an AI-assisted environment, ensuring design decisions satisfy business requirements while providing a solid foundation for AI-assisted implementation.

## Core Principles

The following Vibe Coding core principles should be followed during the design phase:

- **Divide & Conquer for Emergence**: Design "AI-friendly" architecture with clear component boundaries
- **Isomorphic Mapping of Intent**: Ensure high-level design intentions can be mapped to specific components
- **Adaptive Mutation of Explicit Covenants**: Design clear interface contracts while allowing implementation details to evolve

## Practical Steps

### 1. Architectural Vision Building

**Goal**: Create a clear high-level architectural view

**Best Practices**:
- Derive architectural decisions from high-level business goals
- Use visual diagrams to illustrate system components and relationships
- Map non-functional requirements to architectural features
- Leverage AI to explore multiple architectural options

**Anti-patterns**:
- Focusing on technical details too early rather than overall structure
- Lack of clear rationale for architectural decisions
- Ignoring future system evolution needs

**Example Prompt**:
```
Based on [project requirements], I need to design a system architecture. Please:
1. Propose 2-3 viable architectural approaches
2. Analyze the pros and cons of each approach
3. Consider factors like [scalability/performance/security]
4. Recommend the most suitable approach and explain why
```

### 2. AI-Friendly Component Design

**Goal**: Create components with clear boundaries and single responsibilities

**Best Practices**:
- Design components following the single responsibility principle
- Create clear interfaces and data contracts
- Design "testable" component boundaries
- Consider how to make component designs easy for AI to understand and implement

**Anti-patterns**:
- Complex dependencies and circular references between components
- Vague or overly complex interface definitions
- Unclear or overly coupled component responsibilities

**Example Prompt**:
```
For [system component X], I need to design its internal structure:
1. Please propose core interface definitions
2. Design the main data structures
3. Clarify the component's responsibility boundaries
4. Explain how this component interacts with others
5. Consider how to make this design AI-implementation friendly
```

### 3. Design Decision Recording and Consensus

**Goal**: Document key design decisions and their rationale

**Best Practices**:
- Use Architecture Decision Records (ADRs) to document important decisions
- Leverage AI to evaluate design pros and cons and potential risks
- Create design consensus documents as team references
- Establish a review mechanism for design changes

**Anti-patterns**:
- Design decisions not clearly documented
- Lack of rationale explanation for design choices
- Design documents disconnected from actual implementation

**Example Prompt**:
```
For [design decision X], please help me:
1. Summarize the background and constraints that led to this choice
2. List the alternatives we considered
3. Analyze the advantages and potential risks of the current approach
4. Suggest implementation guidelines and considerations
```

### 4. Design Validation and Prototyping

**Goal**: Validate the feasibility and appropriateness of the design

**Best Practices**:
- Create proof of concepts (POCs) for critical parts
- Use AI to generate design validation test cases
- Conduct early performance and scalability evaluations
- Collect and integrate feedback to adjust the design

**Anti-patterns**:
- Skipping validation and moving directly to full implementation
- Ignoring key technical risk points
- Lack of verification for design assumptions

**Example Prompt**:
```
To validate the feasibility of [design approach X], please:
1. Design a minimal viable proof of concept experiment
2. Propose key test scenarios and expected results
3. Analyze potential technical risks and mitigation strategies
4. Suggest key metrics to collect during the validation process
```

## Success Indicators

- Clear design documentation with team consensus
- Well-defined component responsibilities and boundaries
- Key design decisions well-documented
- Design easily decomposable into independently implementable tasks

## IDE Implementation References

- [Cursor Implementation Guide](../ai-ide/cursor/overview.md)
- [Windsurf Implementation Guide](../ai-ide/windsurf/overview.md)

---

## Further Reading

- [Requirements Analysis Best Practices](./requirements.md)
- [Implementation Best Practices](./implementation.md)
- [Divide & Conquer for Emergence Principle](../principles/golden-rules.md#4-divide--conquer-for-emergence)
