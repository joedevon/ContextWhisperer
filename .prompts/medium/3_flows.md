# Medium Codebase Workflow Analysis

## Purpose
Final phase of medium codebase analysis, focusing on understanding key workflows, data flows, and process chains within the system.

## Token Limits
- Maximum per generated file: 3000 tokens
- Recommended split point: 2500 tokens
- Expected number of context files: 2-3

## Analysis Instructions

1. **Core Workflow Identification**
   - Map primary user workflows
   - Document data flow patterns
   - Identify key process chains
   - Note system entry points

2. **Integration Flow Analysis**
   - Document service interactions
   - Map API flows and dependencies
   - Identify cross-component workflows
   - Note external system dependencies

3. **Process Chain Documentation**
   - Document build and deployment flows
   - Map test execution chains
   - Identify data processing pipelines
   - Note error handling flows

4. **Output Format**

Generate a workflows.md file containing:

```markdown
# System Workflows and Processes

## Core Workflows
[Document main user and system workflows]

## Data Flows
[Map key data movement and transformations]

## Integration Points
[Document system interactions and dependencies]

## Process Chains
[Describe key process sequences]

## Error Handling
[Document error flows and recovery processes]
```

5. **Final Integration**
   - Connect workflows to identified patterns
   - Link to structural components
   - Note cross-cutting concerns

## Constraints
- Build upon previous structure and pattern analysis
- Focus on dynamic aspects of the system
- Include sequence diagrams where helpful
- Document error handling and edge cases 