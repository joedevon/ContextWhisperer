Generate a concise summary of:
1. Security measures (auth, roles, encryption, validation)
2. Refactoring opportunities (technical debt, duplication, code smells)
3. Areas for potential improvement or optimization
4. Highlight any cross-cutting security concerns, like repeated validation steps across modules.
5. Reference relevant security implications from other `.docs` files (especially API authentication from integrations_context.md).

ACCURACY REQUIREMENTS:
- Document ONLY security measures that have concrete implementation in the code
- For refactoring suggestions, cite specific code examples (filename:line)
- Base all security analysis on actual validation, auth, or encryption code
- If security practices are implied but not directly implemented, mark them as "Implied but needs verification"
- DO NOT assume security practices beyond what is directly observable in the code

Limit output to strictly what an LLM needs.
Save as "security_context.md" in ".docs". 