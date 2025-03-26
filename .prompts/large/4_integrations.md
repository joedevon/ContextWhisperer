# Large Codebase Integration Analysis

## Purpose
Fourth phase of large codebase analysis, focusing on system integrations, external dependencies, and interface boundaries.

## Token Limits
- Maximum per generated file: 4000 tokens
- Recommended split point: 3500 tokens
- Expected number of context files: 2-4

## Analysis Instructions

1. **External Dependencies**
   - Map third-party integrations
   - Document API dependencies
   - Identify service boundaries
   - Note system interfaces

2. **Integration Patterns**
   - Analyze communication patterns
   - Document data exchange formats
   - Map authentication flows
   - Note error handling

3. **System Boundaries**
   - Document entry points
   - Map exit points
   - Identify boundary interfaces
   - Note cross-system flows

4. **Output Format**

Generate an integrations.md file containing:

```markdown
# System Integrations

## External Dependencies
[Map third-party systems and APIs]

## Integration Patterns
[Document communication patterns]

## System Boundaries
[Describe interface points]

## Data Exchange
[Map data formats and flows]

## Security & Auth
[Document security patterns]
```

5. **Next Steps**
   - Flag workflow dependencies
   - Note performance implications
   - Identify security concerns
   - Mark reliability issues

## Constraints
- Focus on external interfaces
- Document integration patterns
- Include security considerations
- Note reliability concerns 