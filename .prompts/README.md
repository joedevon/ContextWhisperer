# Using Context Whisperer Prompts

This directory contains the core prompt templates that power Context Whisperer. Here's how to use them effectively:

## Directory Structure

- `llm/` - Prompts that generate concise, optimized context for LLMs (extension: `.llm`)
- `human/` - Prompts that generate human-readable documentation (extension: `.hdoc`)

## Usage Instructions

1. Review the prompt templates in this directory
2. Execute prompts by feeding them to your preferred AI coding assistant
3. For context management:
   - Use `./prompts/llm/*.llm` files when your context window gets too large
   - Start a new chat and reference generated `.docs` files for context
4. For documentation:
   - Use `./prompts/human/*.hdoc` files to generate/update documentation
   - Find generated docs in `docs/ai-generated/`

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