# Codebase Improvement Opportunities

This template analyzes the codebase to identify potential improvements and next steps for developers.

ACCURACY REQUIREMENTS:
- Base ALL suggestions on verifiable code evidence
- Focus on concrete, actionable improvements
- Mark uncertainties as "Potentially Missing Information"

1. Identify and categorize improvement opportunities:
   - Technical debt (complex code, workarounds, outdated patterns)
   - Bugs and defects (with evidence from code or tests)
   - Code duplication (with specific duplicate examples)
   - Code smells (overly complex methods, inappropriate dependencies)
   - Architectural issues (antipatterns, scalability concerns)
   - Explicit TODOs in code comments (prioritized by importance)
   - Features mentioned in documentation but not implemented

2. For each improvement opportunity, provide:
   - Description of the issue
   - Code location and evidence
   - Potential impact if addressed/left unaddressed
   - Estimated complexity to fix (Easy, Medium, Hard)
   - Suggested approach to resolve

3. Group and prioritize improvements by:
   - Priority tier:
     - Tier 1: Critical/quick wins (high impact, low effort)
     - Tier 2: Important improvements (high impact, higher effort)
     - Tier 3: Nice-to-have enhancements (lower impact)
   - Category (technical debt, bugs, etc.)
   - Component or subsystem

STRUCTURE FORMAT:
Follow the scaffold.template guidance for document structure:
- Use the standard document structure format specified in the template
- Organize information in a logical progression from highest to lowest priority
- Include practical examples with file references

OUTPUTS:
1. Save the main document as "future_doc.md" in "docs/ai-generated/"

PREFERENCES:
- Follow all settings in the preferences.config file for formatting, environment, and style choices
- Use terminal command formats based on the shell specified in preferences
- Match the specified code style preferences for any code snippets
- Adhere to the documentation style and content preferences 