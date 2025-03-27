# Using Context Whisperer Prompts

This directory contains prompt templates for enhancing AI-assisted development. While the core focus is on context management, the architecture supports various development workflows.

## Directory Structure

- `llm/` - Prompts that generate concise, optimized context for LLMs (extension: `.llm`)
- `human/` - Prompts that generate human-readable documentation (extension: `.hdoc`)
- `utility/` - General-purpose development prompts
  - `.cursor` - Prompts optimized for Cursor IDE
  - `.windsurf` - Prompts optimized for WindSurf (coming soon)
  - `.claude` - Prompts optimized for Claude Code (coming soon)
  - Git workflows, code review, and other development tasks

## Usage Instructions

1. Review the prompt templates in this directory
2. Execute prompts by feeding them to your preferred AI coding assistant
3. For context management:
   - Use `./prompts/llm/*.llm` files when your context window gets too large
   - Start a new chat and reference generated `.docs` files for context
4. For documentation:
   - Use `./prompts/human/*.hdoc` files to generate/update documentation
   - Find generated docs in `docs/ai-generated/`
5. For utility prompts:
   - Choose prompts with the extension matching your IDE/assistant
   - Each IDE version is optimized for that environment's specific features
   - Core functionality remains similar across versions

## Output Locations

- LLM prompts (`.llm`) → `.docs/` directory
- Human prompts (`.hdoc`) → `docs/ai-generated/` directory

## Prompt Categories and Order

### LLM Prompts (`llm/`)
- `0.prep_add_inline_comments.llm` - Adds comments to code (no output file)
- `1.core_architecture_and_domain.llm` - Core architecture and domain concepts
- `2.ops_operations.llm` - Operational aspects
- `3.ext_apis_and_extensions.llm` - APIs and extension points
- `4.ext_security_and_refactoring.llm` - Security and refactoring opportunities

### Human Prompts (`human/`)
- `1.architecture_overview.hdoc` - Detailed architecture explanation
- `2.onboarding_guide.hdoc` - Developer onboarding documentation
- `3.component_documentation.hdoc` - Component-level documentation
- `4.workflows_and_processes.hdoc` - Business workflows and processes
- `5.troubleshooting_guide.hdoc` - Common issues and solutions 