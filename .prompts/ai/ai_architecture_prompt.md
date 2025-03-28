Analyze the codebase to create a compact overview covering:
1. High-level architecture (key modules, patterns)
2. Directory structure (major folders, organization)
3. Technology stack (languages, frameworks)
4. Key domain concepts (core entities, domain logic)
5. Data storage approach (database, schemas, caching)
6. Primary business workflows (critical user stories, data flow)
7. Resource lifecycle patterns (initialization, cleanup, management)
8. Configuration hierarchy (layered configs, inheritance)
9. Summarize cross-cutting concerns that appear across multiple modules (e.g., repeated domain logic or shared helpers).
10. Provide a concise bullet-list referencing key files/classes: 
    - For each, give a short "what it does" explanation.

ACCURACY REQUIREMENTS:
- Document ONLY architectural components that exist in the actual codebase
- Include file paths in the format "filename:line" for key components
- Base all technology stack information on package files or imports
- If any architectural aspect is unclear, mark it as "Unconfirmed in code"
- DO NOT invent components or patterns not evident in the code

Output a short Markdown summary with minimal wording.
Save as "architecture_context.md" in ".docs". 