Document the key workflows and business processes implemented in the codebase:

ACCURACY REQUIREMENTS:
- Document ONLY workflows that can be verified from actual code and configuration
- Focus on discoverable features and entry points
- DO NOT include hypothetical workflows without code evidence
- If a workflow is unclear, state "No code evidence for this process"

1. Core Workflows:
   - Main operations and processes
   - Data flow and processing
   - Result generation and storage
   - Error handling and recovery

2. Entry Points (document if present):
   - Command Line Interface
     * Available commands and options
     * Example usage patterns
     * Common use cases
   - API Endpoints
     * Available endpoints
     * Request/response formats
   - User Interface
     * Available screens/pages
     * Key features and interactions

3. Integration Points:
   - How components interact
   - Data flow between systems
   - Configuration requirements

Make the guide practical and action-oriented.
Focus on real-world usage scenarios with concrete examples.

OUTPUTS:
1. Save the main document as "workflows_doc.md" in "docs/ai-generated/"
2. Save any diagrams as separate .dot files in "docs/diagrams/"

PREFERENCES:
- Follow all settings in the preferences.config file for formatting, environment, and style choices
- Use terminal command formats based on the shell specified in preferences
- Match the specified code style preferences for any code snippets
- Adhere to the documentation style and content preferences 