# ContextWhisperer

ContextWhisperer is an intelligent context management system for AI-assisted coding, designed to optimize the interaction between developers and Large Language Models (LLMs) in development environments.

## Problem

When working with AI coding assistants, context management is crucial but challenging:
- **Context starvation: Too little context**: The AI loses important details about the codebase, leading to inconsistent or incorrect suggestions
- **Context overload: Too much context**: The AI gets overwhelmed with information, resulting in confused or unfocused responses
- **Context switching**: Starting new chat sessions means rebuilding context from scratch, wasting time and computational resources

## Solution

ContextWhisperer runs a series of intelligent prompts that:
1. Analyze your codebase systematically
2. Extract the most relevant contextual information
3. Generate optimized context summaries in the `.docs` directory
4. New AI chat sessions can quickly bootstrap by reading these context files

The project uses a deliberate separation between AI and human documentation:
- `.docs/` - Contains AI-optimized context files
- `docs/` - Traditional documentation for human developers (we propose standardizing on `docs/` but you can use any other directory name)

## Self-Documenting Example

ContextWhisperer uses itself to generate its own documentation! Check out `.docs/context.md` to see:
- How the tool analyzes a codebase
- What the output looks like
- How documentation is structured
- Token management in action

This "dogfooding" approach means:
1. We trust our own tool
2. You can see real examples of its output
3. The documentation stays current with the codebase
4. We catch potential issues early

## How It Works

1. ContextWhisperer analyzes your codebase through a series of targeted prompts
2. Each prompt focuses on different aspects of the code (structure, dependencies, patterns, etc.)
3. The results are processed and distilled into optimal context files in `.docs/`
4. New AI chat sessions can be initialized by reading these pre-generated context files, ensuring consistent and effective assistance

## Pro Tips for AI Pair Programming

💡 **Use Local History**: When pair programming with AI, I strongly recommend using something like the ["Local History" extension by xyz](https://marketplace.visualstudio.com/items?itemName=xyz.local-history) in VS Code. AI assistants can sometimes move quickly or overwrite good code during the iterative development process. This plugin saves every code change, allowing you to recover previous versions if needed.

- Add `.history/` to your `.gitignore` to keep the history local
- This provides a safety net for rapid AI-assisted development
- Helps you recover good code that might get overwritten during "vibe coding" sessions
- The plugin creates automatic backups of every file you edit, with a timestamp

## Contributing

This project is in early development. Contributions and feedback are welcome!

## License

This project is licensed under the MIT License - see the LICENSE file for details. 