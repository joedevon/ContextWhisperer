# Context Whisperer Prompts

This directory contains prompts for generating context and documentation:

## Directory Structure

- `llm/` - Prompts that generate concise, optimized context for LLMs (extension: `.llm`)
- `human/` - Prompts that generate human-readable documentation (extension: `.hdoc`)

## How to Use

1. When your context window gets too large, use the `./prompts/llm/x.category_name.llm` file(s) to generate concise documentation designed for LLMs.
2. Then start a new chat and use the `.docs` generated files to feed the appropriate context to the new context window.
3. If you want updated human-readable documentation, use the `./prompts/human/x.category_name.hdoc` file(s) to generate the updated documentation in the `./docs/ai-generated` directory.

## Output Locations

- LLM prompts (`.llm`) output to the `.docs/` directory
- Human prompts (`.hdoc`) output to the `docs/ai-generated/` directory

## Prompt Naming Convention

Both directories use numbered prompts to suggest execution order:

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