# Context Whisperer

> **ContextWhisperer is an intelligent context management system for AI-assisted coding, designed to optimize the interaction between developers and Large Language Models (LLMs) in development environments.**

## Origin & Philosophy

ContextWhisperer emerged from experiencing the limitations of automated system prompts in AI coding assistants. While using cursorrules (system prompts), I noticed that over time, these automated prompts would accumulate stale context and become increasingly complex, leading to confused LLM responses. The solution became clear: replace automated system prompts with intentional, task-specific context management.

Instead of relying on complex automated rules, ContextWhisperer uses manual, targeted prompts to generate fresh, relevant context when needed. This approach enables a powerful workflow: dedicate each context window to a single, focused task. Don't fear starting fresh windows - simply run the relevant prompts to bootstrap your new context with clean, current, LLM-optimized information about your codebase. This "fresh start" approach leads to clearer communication with AI assistants and better results.

## Problem

When working with AI coding assistants, context management is crucial but challenging:
- **Context starvation: Too little context**: The AI loses important details about the codebase, leading to inconsistent or incorrect suggestions
- **Context overload: Too much context**: The AI gets overwhelmed with information, resulting in confused or unfocused responses
- **Context switching**: Starting new chat sessions means rebuilding context from scratch, wasting time and computational resources

## Solution

ContextWhisperer provides a series of intelligent prompts that:
1. Analyze your codebase systematically
2. Extract the most relevant contextual information
3. Generate optimized context summaries for both LLMs and humans
4. Enable quick context bootstrapping for new AI chat sessions
5. Provide clear, maintainable documentation for development teams

## Directory Structure

- `.prompts/`: Contains prompt templates that power the system
  - `llm/`: Prompts optimized for LLM context management
  - `human/`: Prompts for generating human documentation
  - `utility/`: General-purpose development prompts (git workflows, code review, etc.)
- `.docs/`: Stores LLM-optimized context files
- `docs/`: Houses human-readable documentation
  - `ai-generated/`: Auto-generated documentation for developers

## Installation

Simply copy the `.prompts` directory into your project root. See `.prompts/README.md` for detailed usage instructions.

## Pro Tips for AI Pair Programming

💡 **Use Local History**: When pair programming with AI, I strongly recommend using something like the ["Local History" extension by xyz](https://marketplace.visualstudio.com/items?itemName=xyz.local-history) in VS Code. AI assistants can sometimes move quickly or overwrite good code during the iterative development process. This plugin saves every code change, allowing you to recover previous versions if needed. Be sure to add the `.history` file to your `.gitignore` file.

💡 **Use TDAID Principles**: I stumbled upon a good pattern for Applying TDD principles to improve LLM-generated code quality and speed. I wrote it up and open sourced it here:

https://github.com/joedevon/TDAID

## Author

### Joe Devon
- 🐦 Social Media: @joedevon
- 🎙️ Podcast: [Accessibility and Gen. AI](https://www.youtube.com/@a11ygenai)
- 📫 Newsletter: [Joe Dev On Tech](https://www.linkedin.com/newsletters/joe-dev-on-tech-7240847501472194560/) - subscribe to get updates on my projects and articles

## Contributing

This project is in early development. Contributions and feedback are welcome!

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.