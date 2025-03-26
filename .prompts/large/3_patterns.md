# Large Codebase Pattern Analysis

## Purpose
Third phase of large codebase analysis, identifying and documenting system-wide patterns, conventions, and architectural decisions.

## Token Limits
- Maximum per generated file: 4000 tokens
- Recommended split point: 3500 tokens
- Expected number of context files: 2-4

## Analysis Instructions

1. **Architectural Patterns**
   - Document major design patterns
   - Identify architectural styles
   - Map cross-cutting patterns
   - Note pattern variations

2. **Code Organization**
   - Analyze module patterns
   - Document package structures
   - Identify layer patterns
   - Map dependency patterns

3. **Development Patterns**
   - Document coding conventions
   - Analyze testing patterns
   - Map build patterns
   - Note deployment patterns

4. **Output Format**

Generate a patterns.md file containing:

```markdown
# System Patterns

## Architectural Patterns
[Document major architectural patterns]

## Design Patterns
[Map recurring design solutions]

## Code Organization
[Describe structural patterns]

## Development Patterns
[Document development conventions]

## Pattern Variations
[Note context-specific adaptations]
```

5. **Next Steps**
   - Flag integration implications
   - Note workflow impacts
   - Identify pattern conflicts
   - Mark maintenance concerns

## Constraints
- Focus on system-wide patterns
- Document pattern rationale
- Include pattern variations
- Note anti-patterns 