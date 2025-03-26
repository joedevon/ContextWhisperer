# Large Codebase Core Component Analysis

## Purpose
Second phase of large codebase analysis, performing deep-dive analysis of core system components identified in the overview phase.

## Token Limits
- Maximum per generated file: 4000 tokens
- Recommended split point: 3500 tokens
- Expected number of context files: 3-5

## Analysis Instructions

1. **Core Component Identification**
   - Analyze primary business logic
   - Document core data models
   - Map critical services
   - Identify essential utilities

2. **Component Dependencies**
   - Map internal dependencies
   - Document component interfaces
   - Analyze coupling patterns
   - Note circular dependencies

3. **Implementation Details**
   - Document key algorithms
   - Analyze data structures
   - Map state management
   - Note performance considerations

4. **Output Format**

Generate a core.md file containing:

```markdown
# Core Components

## Business Logic
[Document primary business components]

## Data Models
[Describe core data structures]

## Critical Services
[Map essential services and their roles]

## Component Dependencies
[Document internal relationships]

## Implementation Notes
[Detail key algorithms and patterns]
```

5. **Next Steps**
   - Flag areas for pattern analysis
   - Note integration points
   - Identify workflow dependencies
   - Mark performance-critical sections

## Constraints
- Focus on business-critical components
- Include implementation details
- Document component interfaces
- Note performance considerations 