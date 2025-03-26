# Medium Codebase Pattern Analysis

## Purpose
Second phase of medium codebase analysis, focusing on identifying and documenting code patterns, conventions, and recurring architectural elements.

## Token Limits
- Maximum per generated file: 3000 tokens
- Recommended split point: 2500 tokens
- Expected number of context files: 2-3

## Analysis Instructions

1. **Code Pattern Identification**
   - Analyze common coding patterns
   - Document design patterns in use
   - Identify architectural patterns
   - Note testing patterns and conventions

2. **Convention Analysis**
   - Document naming conventions
   - Identify file organization patterns
   - Note code style preferences
   - Document common idioms

3. **Anti-Pattern Detection**
   - Identify potential code smells
   - Note areas of technical debt
   - Flag inconsistent patterns
   - Document workarounds and their reasons

4. **Output Format**

Generate a patterns.md file containing:

```markdown
# Code Patterns and Conventions

## Design Patterns
[List and explain key design patterns in use]

## Coding Conventions
[Document standard practices and conventions]

## Architecture Patterns
[Describe recurring architectural elements]

## Testing Patterns
[Document testing approaches and conventions]

## Areas for Improvement
[Note potential technical debt and anti-patterns]
```

5. **Next Steps**
   - Flag areas that need workflow analysis
   - Note patterns that affect system flows
   - Identify integration points

## Constraints
- Build upon structure analysis from phase 1
- Focus on patterns, not individual implementations
- Include examples with file references
- Note pattern variations across different components 