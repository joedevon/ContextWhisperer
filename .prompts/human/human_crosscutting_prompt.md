Create a comprehensive guide to cross-cutting concerns in the codebase:

ACCURACY REQUIREMENTS:
- Base all documentation on actual code implementations
- Compare actual patterns with `llm.yaml` preferences
- Mark any discrepancies as "Implementation Note"

1. Cross-Cutting Patterns Overview:
   - Document each major cross-cutting concern
   - Explain the chosen implementation approach
   - Provide rationale for architectural decisions
   - Note any variations across the codebase

2. Implementation Guide:
   - How to implement new features following patterns
   - Common pitfalls to avoid
   - Best practices and conventions
   - Examples from existing code

3. Pattern Details (for each concern):
   - Configuration and setup
   - Usage examples
   - Integration points
   - Testing requirements

4. Architectural Consistency:
   - Compare actual implementations with `llm.yaml`
   - Document any approved deviations
   - Explain migration plans for inconsistencies
   - Provide guidance for maintaining consistency

Make the guide practical and example-driven.
Focus on helping developers maintain architectural consistency.

OUTPUTS:
1. Save the main document as "crosscutting_doc.md" in "docs/ai-generated/"
2. Save any diagrams as separate .dot files in "docs/diagrams/" 