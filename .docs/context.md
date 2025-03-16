# Project Context

## Overview
ContextWhisperer is a tool designed to solve one of the key challenges in AI-assisted coding: context management. It analyzes codebases and generates optimized context documentation that helps AI assistants understand projects quickly and consistently. The tool prevents both context starvation (too little information) and context overload (too much information) by creating well-structured, size-constrained documentation.

## Structure
[See detailed structure in [tree.md](./tree.md)]

Key directories:
- `.prompts/` - Contains the analysis prompts organized by project size
  - `small/` - Prompts for analyzing small projects
  - (medium and large to be implemented)
- `.docs/` - Contains the AI-optimized context files (you're reading one now!)

## Key Components

### Analysis Prompts
- `small/analyze.md`: Main prompt template for small projects
  - Implements tree-based structure analysis
  - Enforces 2000 token limit per file (1500 recommended split point)
  - Provides file organization strategies
  - Includes guidance for AI conversation management

## Technologies
- Language-agnostic documentation generation
- Uses standard Unix tools (tree)
- Markdown-based documentation
- Designed for use with AI coding assistants (Cursor, etc.)

## Conventions
- Documentation:
  - AI-specific docs in `.docs/`
  - Human docs in user-chosen directory
  - Token limits: 2000 max, split at 1500
  - Always link related documents
- File Organization:
  - Prompts in `.prompts/`
  - Size-based analysis selection
  - Component-based file splitting
- Naming:
  - Clear, descriptive file names
  - Size-prefixed prompt directories (small/, medium/, large/)

## Configuration
No configuration files needed yet. The tool is currently prompt-based.

## Entry Points
1. Install via script:
   ```bash
   curl -L https://raw.githubusercontent.com/joedevon/ContextWhisperer/main/install.sh | bash
   ```
   (Note: Script to be implemented - currently clone the repository)
2. Choose appropriate prompt from `.prompts/` based on project size
3. Run analysis prompt with AI assistant
4. Generated context will be created in `.docs/`

Future plans:
- Implement installation script
- pip package for enhanced features
- medium and large project analysis
- more sophisticated prompt templates

## Meta Note
This context.md file was generated using ContextWhisperer's own small project analysis prompt - a form of dogfooding that demonstrates the tool's capabilities on its own codebase. 