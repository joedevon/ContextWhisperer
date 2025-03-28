# Context Whisperer

> **ContextWhisperer is an intelligent context management system for AI-assisted coding, designed to optimize the interaction between developers and Large Language Models (LLMs) in development environments. This version is optimized for use with Cursor IDE.**

## Quick Start in 3 Steps

1.  Copy the `.prompts` directory into your project root.
2.  **Basic Cursor Workflow:**
    *   **Define Preferences (Recommended):** Either manually edit `llm.yaml` to set your cross cutting architectural preferences, or @ tag `utility/cross_cutting_interview.md` in Cursor chat for an interactive setup.
    *   **Generate Context/Docs:**
        - **For LLM Context:** In the Cursor chat, `@` tag a specific prompt like `.prompts/ai/ai_architecture_prompt.md` OR tag the whole folder `.prompts/ai/` to run all LLM context prompts. Output goes to `.docs/`.
        - **For Human Docs:** In the Cursor chat, `@` tag a specific prompt like `.prompts/human/human_architecture_prompt.md` OR tag the whole folder `.prompts/human/` to run all documentation prompts. Output goes to `docs/ai-generated/`.
    *   **Bootstrap New Chats:** In a new Cursor chat, use `@` references to include context from the entire `.docs/` directory, or focus in on a specific file (e.g., `.docs/architecture_context.md`) to provide focused context.
3.  See `.prompts/README.md` for more detailed instructions on specific prompts and outputs.

## Problem

When working with AI coding assistants, context management is crucial but challenging:
- **Context starvation: Too little context**: The AI loses important details about the codebase, leading to inconsistent or incorrect suggestions
- **Context overload: Too much context**: The AI gets overwhelmed with information, resulting in confused or unfocused responses
- **Context switching**: Starting new chat sessions means rebuilding context from scratch, wasting time and computational resources
- **Cross-cutting inconsistency**: Without persistent understanding of architectural patterns, LLMs often implement cross-cutting concerns (logging, error handling, etc.) inconsistently across sessions

## Solution

ContextWhisperer provides a series of prompts that:
- Interactively guide you to make the architectural decisions about the cross cutting concerns that tend to trip up cursor.
  - These decisions will be saved in an `llm.yaml` file in your project root.
  - You are welcome to edit the `llm.yaml` file directly, or use the prompts to guide you.
- Generate optimized context summaries by running prompts from `.prompts/ai/` (outputting to `.docs/`) and human-readable documentation via prompts in `.prompts/human/` (outputting to `docs/ai-generated/`).
- Enable quick context bootstrapping for new AI chat sessions by referencing the generated `.docs/` files.

## Origin & Philosophy

ContextWhisperer emerged from experiencing the limitations of .cursorrules as a means of combatting the dance between context starvation and overload. I made the rules more complex as issues arose. Before long I forgot what rules are impacting my AI interactions. I got confused, cursor got confused, and the code output degraded.

The devs behind cursor continue trying to improve the rules system, but an [insight](https://simonwillison.net/2025/Mar/11/using-llms-for-code/) by [Simon Willison](https://simonwillison.net/) inspired me to take a different approach.

> One of the reasons I mostly work directly with the ChatGPT and Claude web or app interfaces is that it makes it easier for me to understand exactly what is going into the context. LLM tools that obscure that context from me are less effective.

System prompts that are front and center, can be very useful. But hiding them is an antipattern. It's time to put humans back in control of context management.

Instead of relying on complex automated rules, ContextWhisperer uses manual, targeted prompts to generate fresh, relevant context when needed. This approach enables a powerful workflow: 
- Dedicate each context window to a single, focused task. 
- Don't fear starting fresh context windows - simply run the relevant prompts to bootstrap your new context with clean, current, LLM-optimized information about your codebase. 

This "fresh start" approach leads to clearer communication with AI assistants and better results.

A key part of this philosophy is establishing conventions for how LLMs should handle cross-cutting concerns. When an LLM implements environment variable management, one session might use `.env` files while another implements a secrets manager. What a mess!

By standardizing how we communicate architectural patterns to LLMs, for example using consistent file naming, say `llm.yaml`, and setting preferences with consistent key/value pairs, say `envs: secrets_manager`, or `logging: structured`, LLMs will evolve to look for these configuration patterns, reducing architectural drift over time. 


## Roadmap

- **Core:** Develop the interactive interview prompt (`.prompts/utility/cross_cutting_interview.md`) for guiding users in creating and maintaining their `llm.yaml` file.
- **Future Goal:** Documentation Synchronization
  - Explore potential for smarter README reconciliation using `.docs` context.

## Directory Structure

- `.prompts/`: Contains prompt templates that power the system
  - `ai/`: Prompts optimized for LLM context management
  - `human/`: Prompts for generating human documentation
  - `utility/`: General-purpose development prompts
- `.docs/`: Stores LLM-optimized context files (`*_context.md`)
- `docs/`: Houses human-readable documentation
  - `ai-generated/`: Auto-generated documentation (`*_doc.md`)
- `llm.yaml`: Configuration file storing architectural patterns for cross-cutting concerns

## Pro Tips for AI Pair Programming

💡 **Use Local History**: When pair programming with AI, I strongly recommend using something like the ["Local History" extension by xyz](https://marketplace.visualstudio.com/items?itemName=xyz.local-history) in VS Code. AI assistants can sometimes move quickly or overwrite good code during the iterative development process. This plugin saves every code change, allowing you to recover previous versions if needed. Be sure to add the `.history` file to your `.gitignore` file.

💡 **Use TDAID Principles**: I stumbled upon a good pattern for Applying TDD principles to improve LLM-generated code quality and speed, wrote it up and open sourced it here:

https://github.com/joedevon/TDAID

## Call to Action: Improve ContextWhisperer

If you like this approach, spread the word on social media. Let's use #ContextWhisperer as our hashtag. Feel free to tag the author @joedevon.

## Author

### Joe Devon
- 🐦 Social Media: @joedevon
- 🎙️ Podcast: [Accessibility and Gen. AI](https://www.youtube.com/@a11ygenai)
- 📫 Newsletter: [Joe Dev On Tech](https://www.linkedin.com/newsletters/joe-dev-on-tech-7240847501472194560/) - subscribe to get updates on my projects and articles

## Contributing

This project is in early development. Contributions and feedback are welcome!

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.