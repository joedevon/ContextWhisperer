# Using Context Whisperer Prompts

This directory contains prompt templates for enhancing AI-assisted development, focusing on context management and consistent architectural patterns.

## Directory Structure

- `ai/` - Prompts that generate concise, optimized context for LLMs
  - Output files go to `.docs/` with `*_context.md` naming pattern
  - Example: `ai_architecture_prompt.md` → `.docs/architecture_context.md`

- `human/` - Prompts that generate human-readable documentation
  - Output files go to `docs/ai-generated/` with `*_doc.md` naming pattern
  - Example: `human_architecture_prompt.md` → `docs/ai-generated/architecture_doc.md`

- `utility/` - General-purpose development prompts
  - `cross_cutting_interview.md` - Interactive setup for `llm.yaml`
  - `add_inline_comments.md` - Adds AI-focused context
  - `readme_reconciliation.md` - Detects architectural drift
  - Other utility prompts for git workflows, code review, etc.

## Usage Instructions

1. Configure Cross-Cutting Concerns:
   - Run `utility/cross_cutting_interview.md` to set up `llm.yaml`
   - This ensures consistent handling of logging, error handling, etc.

2. Prepare Codebase Context:
   - Run `utility/add_inline_comments.md` to add AI-focused inline comments
   - This helps LLMs understand architectural decisions and patterns
   - Focus on documenting cross-cutting concerns implementation

3. Generate LLM Context:
   - Use prompts in `ai/*.md` to generate optimized context
   - Context files are saved in `.docs/` directory
   - Reference these in new chat sessions for consistent context

4. Generate Human Documentation:
   - Use prompts in `human/*.md` to generate documentation
   - Docs are saved in `docs/ai-generated/`

5. Monitor Architectural Drift:
   - Run `utility/readme_reconciliation.md` periodically
   - Compares actual implementation (`crosscutting_context.md`) with desired patterns (`llm.yaml`)
   - Helps identify inconsistencies in cross-cutting concerns

## Available Prompts

### AI Context Prompts
- `ai_architecture_prompt.md` - Core architecture and patterns
- `ai_operations_prompt.md` - Operational aspects
- `ai_integrations_prompt.md` - External APIs and integrations
- `ai_security_prompt.md` - Security measures and improvements
- `ai_crosscutting_prompt.md` - Actual cross-cutting implementations

### Human Documentation Prompts
- `human_architecture_prompt.md` - Detailed architecture docs
- `human_onboarding_prompt.md` - Developer onboarding
- `human_components_prompt.md` - Component documentation
- `human_workflows_prompt.md` - Business workflows
- `human_troubleshooting_prompt.md` - Common issues and solutions
- `human_future_prompt.md` - Future improvements
- `human_crosscutting_prompt.md` - Cross-cutting patterns guide

### Utility Prompts
- `cross_cutting_interview.md` - Interactive `llm.yaml` setup
- `add_inline_comments.md` - Add AI-focused context
- `readme_reconciliation.md` - Detect architectural drift
- `commit_msg.cursor.md` - Git commit message helper

## Powered by ContextWhisperer

[ContextWhisperer](https://github.com/joedevon/contextwhisperer) is a project by [Joe Devon](https://linkedin.com/in/joedevon). It's open source and free to use.

If you like it, please star the repo.