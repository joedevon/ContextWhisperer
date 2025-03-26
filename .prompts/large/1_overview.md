# Large Codebase Overview Analysis

## Purpose
Initial phase of large codebase analysis, providing a high-level scan of the system to guide deeper analysis phases.

## Token Limits
- Maximum per generated file: 4000 tokens
- Recommended split point: 3500 tokens
- Expected number of context files: 2-3

## Analysis Instructions

1. **System Boundary Analysis**
   - Identify system scope
   - Map major subsystems
   - Document external interfaces
   - Note system dependencies

2. **Architecture Overview**
   - Document high-level architecture
   - Identify key architectural decisions
   - Map major components
   - Note cross-cutting concerns

3. **Technology Stack**
   - List primary technologies
   - Document framework usage
   - Identify key libraries
   - Note infrastructure components

4. **Output Format**

Generate an overview.md file containing:

```markdown
# System Overview

## System Context
[High-level description of system purpose and scope]

## Architecture Overview
[Document major architectural components]

## Technology Stack
[List and describe key technologies]

## System Boundaries
[Map system interfaces and dependencies]

## Key Decisions
[Document major architectural decisions]
```

5. **Next Steps**
   - Flag core components for deep dive
   - Note areas needing pattern analysis
   - Identify integration points
   - Mark key workflow areas

## Constraints
- Stay high-level - details come in later phases
- Focus on system-wide concerns
- Include architecture diagrams
- Note areas needing deeper analysis 