# Maintenance Best Practices

*AI-assisted refactoring, debugging, and documentation*

[English](../../en/playbooks/maintenance.md) | [中文](../../zh/playbooks/maintenance.md)

## Overview

As software projects evolve, the maintenance phase often consumes the majority of development time and resources. Vibe Coding offers significant advantages in this phase, helping developers more efficiently understand, debug, refactor, and document existing codebases. This guide introduces how to effectively utilize human-machine collaboration during the maintenance phase to improve efficiency and maintain code quality.

## Core Principles

The following Vibe Coding core principles should be followed during the maintenance phase:

- **Memory & Navigation**: Utilize AI to quickly understand complex codebases
- **Closed-Loop Autonomy of Quality Calibration Circuits**: Maintain and improve code quality through continuous feedback
- **Adaptive Mutation of Explicit Covenants**: Optimize implementations while maintaining stable interfaces
- **Proactive Resilience Engineering**: Enhance the system's ability to adapt to changes

## Practical Steps

### 1. Code Understanding and Context Building

**Goal**: Quickly understand the structure and intent of existing code

**Best Practices**:
- Use AI to analyze codebase structure and component relationships
- Create flowcharts and dependency diagrams for key functionalities
- Identify design patterns and architectural decisions
- Build a code knowledge base, documenting the purpose and interactions of key components

**Anti-patterns**:
- Making changes without sufficient understanding of the code
- Focusing only on code fragments while ignoring the overall architecture
- Not recording key findings for future reference

**Example Prompt**:
```
Please help me analyze this [module/class/function]:
1. Summarize its main functionality and responsibilities
2. Identify key design patterns or architectural features
3. Explain how it interacts with other components
4. Highlight potential areas for improvement or risk
```

### 2. Precise Debugging and Problem Diagnosis

**Goal**: Efficiently locate and resolve code issues

**Best Practices**:
- Provide detailed problem descriptions and context
- Use AI to analyze potential failure points and root causes
- Create minimized reproduction cases
- Verify the effectiveness and side effects of solutions

**Anti-patterns**:
- Providing vague problem descriptions
- Implementing "band-aid" fixes without addressing root causes
- Neglecting comprehensive testing validation

**Example Prompt**:
```
I'm experiencing [specific issue], with the following information:
- Error message: [error log/stack trace]
- Reproduction steps: [detailed steps]
- Related code: [code snippet]
- Solutions already attempted: [previous attempts]

Please help me:
1. Analyze possible causes
2. Suggest specific debugging strategies
3. Recommend solutions
```

### 3. Safe Refactoring and Code Optimization

**Goal**: Improve code quality while maintaining system stability

**Best Practices**:
- Clearly define refactoring goals and scope
- Follow the "modify source code only when necessary" principle
- Establish automated testing safeguards
- Perform incremental refactoring with small commits
- Document refactoring decisions and trade-offs

**Anti-patterns**:
- Large-scale refactoring without adequate test coverage
- Mixing feature changes with refactoring
- Failing to assess performance after refactoring

**Example Prompt**:
```
I need to refactor [specific code] to address [specific issue]. Please:
1. Propose an incremental refactoring strategy
2. Design test plans for each refactoring step
3. Evaluate potential risks and side effects
4. Suggest validation measures after refactoring
```

### 4. Technical Debt Management

**Goal**: Systematically identify and address technical debt

**Best Practices**:
- Use AI to identify technical debt in the codebase
- Categorize and prioritize technical debt
- Create sustainable technical debt repayment plans
- Balance new feature development with debt repayment

**Anti-patterns**:
- Ignoring accumulated technical debt
- Lack of visibility and quantification of technical debt
- Focusing only on new features without allocating resources for debt management

**Example Prompt**:
```
Please help me analyze technical debt in [codebase/module]:
1. Identify major code quality issues (complexity, duplication, outdated patterns, etc.)
2. Assess the severity and fix cost of each issue
3. Suggest a prioritized list of issues to address
4. Propose an incremental improvement strategy
```

### 5. Documentation Updates and Knowledge Management

**Goal**: Maintain synchronization between documentation and code, capture knowledge

**Best Practices**:
- Use AI to generate and update technical documentation
- Establish a "living documentation" system that evolves with code changes
- Record key decisions and problem solutions
- Create a repository of common issues and solutions

**Anti-patterns**:
- Documentation updates lagging behind code changes
- Knowledge existing only with individuals rather than shared with the team
- Lack of capture of important experiences

**Example Activities**:
- Regularly use AI to review consistency between documentation and code
- Create knowledge base entries for key issues and solutions
- Establish links between code comments and external documentation

## Success Indicators

- Shortened problem resolution time
- Continuously improving code quality metrics
- Improved documentation completeness and timeliness
- Increased knowledge sharing and reuse rate

## IDE Implementation References

- [Cursor Implementation Guide](../ai-ide/cursor/overview.md)
- [Windsurf Implementation Guide](../ai-ide/windsurf/overview.md)

---

## Further Reading

- [Implementation Best Practices](./implementation.md)
- [Closed-Loop Autonomy of Quality Calibration Circuits Principle](../principles/golden-rules.md#10-closed-loop-autonomy-of-quality-calibration-circuits)
