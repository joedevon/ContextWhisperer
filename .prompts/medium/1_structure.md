# Medium Codebase Structure Analysis

## Purpose
This is the first phase of analyzing a medium-sized codebase. It focuses on understanding the overall structure and organization of the project.

## Token Limits
- Maximum per generated file: 3000 tokens
- Recommended split point: 2500 tokens
- Expected number of context files: 2-4

## Analysis Instructions

1. **Directory Structure Analysis**
   - Generate a comprehensive tree view of the project
   - Identify main components and their relationships
   - Document key configuration files and their purposes
   - Note any unusual or non-standard directory structures

2. **Component Organization**
   - Map primary code components
   - Document module boundaries
   - Identify shared resources and utilities
   - Note testing and documentation organization

3. **File Classification**
   - Group files by their roles (core logic, utilities, tests, etc.)
   - Identify configuration and build files
   - Document resource files and assets
   - Note any generated code or build artifacts

4. **Output Format**

Generate a structure.md file containing:

```markdown
# Project Structure

## Overview
[High-level description of project organization]

## Directory Structure
[Annotated tree view with key components]

## Component Map
[Description of main components and their relationships]

## Configuration
[Key configuration files and their purposes]

## Resource Organization
[How shared resources and assets are managed]
```

5. **Next Steps**
   - Flag areas that need deeper pattern analysis
   - Note potential architectural patterns for phase 2
   - Identify workflow-heavy areas for phase 3

## Constraints
- Focus on structure only - leave patterns and workflows for later phases
- Keep descriptions concise and AI-optimized
- Include relevant file paths for all components
- Link to other context files when splitting 