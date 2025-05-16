# Windsurf Workflow Patterns

*Best practices for Windsurf workflow configuration and usage*

[English](../../../en/ai-ide/windsurf/workflows/workflow-patterns.md) | [中文](../../../zh/ai-ide/windsurf/workflows/workflow-patterns.md)

## Workflow System Overview

Windsurf's workflow system allows for creating predefined sequences of operations, standardizing and automating common tasks. It is an important tool for implementing the Vibe Coding principles of "Fidelity & Amplification of Value Stream" and "Iterative Evolutionary Engine."

Workflows are stored as Markdown files in the `.windsurf/workflows/` directory and can be triggered using slash commands (e.g., `/workflow-name`).

## Workflow Design Principles

### 1. Single Responsibility

Each workflow should focus on a single type of task or process:
- Avoid creating overly broad or multi-functional workflows
- Prioritize designing small, composable workflows rather than large monolithic processes
- Clearly define the workflow's inputs, expected outputs, and success criteria

### 2. Standardization and Consistency

Workflows should standardize common team operations:
- Adopt consistent naming and structural conventions
- Conform to project terminology and process standards
- Include clear usage instructions and examples

### 3. Progressive Feedback

Design workflows that support iterative improvement:
- Break complex tasks into verifiable steps
- Provide checkpoints and feedback opportunities at critical nodes
- Support adjusting subsequent steps based on intermediate results

### 4. Maintainability

Ensure workflows are easy to understand and maintain:
- Include sufficient comments and explanations
- Clearly specify the workflow's applicable scenarios and limitations
- Regularly review and update workflows to adapt to project evolution

## Common Workflow Patterns

### 1. Code Review Workflow

**File**: `.windsurf/workflows/code-review.md`

```markdown
---
description: Standardized code review process
---

# Code Review Workflow

## Step 1: Code Overview Analysis
I will analyze the current file or specified code, providing an overall structure and functionality overview.

Please specify the code range to review: [user input file path or range]

## Step 2: Code Quality Assessment
I will assess code quality from the following dimensions:
- Code readability and style
- Potential performance issues
- Security concerns
- Maintainability considerations
- Consistency with project standards

## Step 3: Specific Improvement Suggestions
Based on the issues found, I will provide specific improvement suggestions, including:
- Code examples and refactoring suggestions
- Priority ordering
- Implementation recommendations

## Step 4: Final Checklist
Confirm that all key points have been considered:
- Are edge cases handled?
- Is error handling complete?
- Is documentation sufficient?
- Is test coverage adequate?
```

**Usage Scenarios**:
- Self code review before submission
- Peer code review assistance
- Code quality guidance for new team members

### 2. Requirements Refinement Workflow

**File**: `.windsurf/workflows/requirement-refinement.md`

```markdown
---
description: Convert high-level requirements into structured, actionable requirements
---

# Requirements Refinement Workflow

## Step 1: Initial Requirement Description
Please describe your initial requirement: [user input requirement]

## Step 2: Clarify Key Information
I will ask clarifying questions to refine the requirement:
- Specific target users and usage scenarios
- Feature boundaries and constraints
- Success criteria and acceptance conditions
- Technical and business limitations
- Priorities and dependencies

## Step 3: Requirement Structuring
I will help organize the requirement into a structured format:
- User story or feature description
- Acceptance criteria
- Non-functional requirements
- Assumptions and constraints
- Risks and mitigation measures

## Step 4: Requirement Confirmation and Memorization
I will provide the final structured requirement and suggest creating a memory to persistently store this information.
```

**Usage Scenarios**:
- Initial requirement discussion and clarification
- User story writing and refinement
- Requirement document standardization

### 3. Technical Design Workflow

**File**: `.windsurf/workflows/technical-design.md`

```markdown
---
description: Create a technical design solution for a new feature or component
---

# Technical Design Workflow

## Step 1: Requirements and Background
Please describe the feature to be designed and its background: [user input]

## Step 2: Design Considerations and Constraints
I will help you think through key design factors:
- Performance requirements and scalability
- Security and compliance
- Integration with existing systems
- Technology stack and limitations
- Maintainability and testing requirements

## Step 3: Design Options Exploration
I will provide 2-3 viable design options, analyzing each one's:
- Advantages and disadvantages
- Implementation complexity
- Risks and mitigation measures
- Resource requirements

## Step 4: Design Decision and Documentation
We will determine the final design approach and create detailed documentation:
- Component structure and interactions
- API design and data model
- Sequence diagrams or flowcharts
- Key algorithms or logic
- Testing strategy

## Step 5: Design Memory Creation
I will help create a memory of the design decision for team reference and future tracking.
```

**Usage Scenarios**:
- Design phase for new features or components
- Solution design before refactoring
- Technology selection and evaluation

### 4. Debugging Assistant Workflow

**File**: `.windsurf/workflows/debugging-assistant.md`

```markdown
---
description: Systematic debugging of complex problems
---

# Debugging Assistant Workflow

## Step 1: Problem Description
Please describe in detail the problem you are experiencing: [user input]

## Step 2: Information Collection
I will guide you in collecting key information:
- Error messages and logs
- Reproduction steps and frequency
- Environment information
- Related code snippets
- Recent code changes

## Step 3: Root Cause Analysis
I will help analyze potential root causes:
- Identify possible failure points
- Suggest methods to validate hypotheses
- Eliminate common causes
- Recommend debugging strategies

## Step 4: Solution
Based on root cause analysis, I will provide:
- Solution suggestions
- Implementation steps
- Verification methods
- Suggestions for preventing similar problems

## Step 5: Knowledge Capture
I will help document the problem and solution to:
- Create troubleshooting guides
- Update project documentation
- Establish memories for future reference
```

**Usage Scenarios**:
- Systematic debugging of complex bugs
- Performance issue investigation
- Production environment incident analysis

## Advanced Workflow Features

### 1. Workflow Composition

Building complex processes by combining small, specialized workflows:

```markdown
---
description: End-to-end process from requirements to implementation
---

# Feature Development Process

## Step 1: Requirements Refinement
/requirement-refinement

## Step 2: Technical Design
/technical-design

## Step 3: Implementation Planning
/implementation-planning

## Step 4: Test Strategy
/test-strategy
```

### 2. Conditional Steps and Branching

Adjusting workflow paths based on intermediate results:

```markdown
## Step 2: Complexity Assessment
I will assess the task complexity:
- If it's a simple task (estimated <2 hours), continue to Step 3A
- If it's a complex task (estimated >2 hours), continue to Step 3B

## Step 3A: Direct Implementation (Simple Task)
...

## Step 3B: Detailed Decomposition (Complex Task)
...
```

### 3. Automation Integration

Integrating workflows with external tools and commands:

```markdown
## Step 4: Run Tests
// turbo
I will run automated tests and analyze the results:
```shell
npm test
```

## Step 5: Code Analysis
// turbo
I will run static code analysis:
```shell
npm run lint
```
```

## Workflow Maintenance and Evolution

### Workflow Governance

Establish mechanisms for managing and updating workflows:

1. **Regular Reviews**:
   - Evaluate workflow usage frequency and effectiveness
   - Collect user feedback and improvement suggestions
   - Ensure alignment with current project practices

2. **Version Control**:
   - Record significant workflow changes
   - Notify the team before updates
   - Maintain backward compatibility or provide clear migration paths

3. **Workflow Directory**:
   - Create a searchable workflow directory
   - Provide clear descriptions and usage examples for each workflow
   - Categorize by domain or application scenario

### Best Practice Sharing

Encourage team sharing and workflow improvement:

1. **Workflow Contribution Guidelines**:
   - Provide templates and guidelines for workflow creation
   - Establish a workflow review process
   - Encourage team members to create domain-specific workflows

2. **Use Case Documentation**:
   - Document successful workflow application cases
   - Share how workflows solved specific challenges
   - Quantify efficiency improvements from workflows

---

Through systematic application of these workflow patterns, you can significantly improve development efficiency, reduce repetitive work, standardize processes, and support core Vibe Coding principles such as "Fidelity & Amplification of Value Stream" and "Closed-Loop Autonomy of Quality Calibration Circuits."
