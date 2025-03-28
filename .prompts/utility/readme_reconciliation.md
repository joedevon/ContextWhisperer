# README Reconciliation Prompt

Purpose: Identify discrepancies between intended design (manually written README files and llm.yaml) and actual implementation (reflected in .docs), facilitating informed decisions about whether to update code or documentation.

## Analysis Phase
1. Extract design intent from:
   a) Manually written README files:
      - Overall architectural intentions
      - Design patterns
      - Project structure
   
   b) llm.yaml:
      - Cross-cutting concern specifications
      - Architectural preferences
      - Implementation standards
   
2. Extract from .docs:
   - Actual implementation patterns
   - Current cross-cutting implementations
   - Technical realities

3. Generate Discrepancy Report:
   ```markdown
   # Implementation vs. Intent Analysis
   
   ## Architectural Patterns
   - Pattern X:
     - Intent (README): [description]
     - Reality (.docs): [description]
     - Impact: [High/Medium/Low]
   
   ## Cross-cutting Concerns
   - Concern Y:
     - Intent (llm.yaml): [specific configuration]
     - Reality (.docs): [description]
     - Impact: [High/Medium/Low]
     - Affected Areas: [list of implementations]
   ```

## Interactive Resolution
For each significant discrepancy:

1. Present Context:
   ```
   Discrepancy found in [area]:
   - Intended design:
     * From README: [description if applicable]
     * From llm.yaml: [configuration if applicable]
   - Current implementation (from .docs): [description]
   ```

2. Query Developer:
   "This difference could indicate either:
    a) Implementation drift that needs correction (code needs to be updated to match README/llm.yaml)
    b) Intentional evolution that should be documented (README/llm.yaml needs to be updated)
    
    Which is it in this case?"

3. Based on response:
   - If (a): Add to Implementation TODOs
   - If (b): Add to Documentation Updates

## Action Plan Generation
Based on all decisions:

1. Implementation TODOs:
   ```markdown
   # Code Updates Needed
   
   ## High Priority
   - [ ] [Description of change needed]
     - Current state: [.docs description]
     - Target state: [README/llm.yaml description]
     - Files affected: [list]
     - Cross-cutting impact: [Yes/No]
   
   ## Medium Priority
   - [ ] [Similar format...]
   ```

2. Documentation Updates:
   ```markdown
   # Documentation Updates Needed
   
   ## README Changes
   - [ ] Update [section] to reflect new [pattern/approach]
     - Old description: [...]
     - New reality: [...]
   
   ## llm.yaml Updates
   - [ ] Update [cross-cutting concern] configuration
     - Current setting: [...]
     - New setting: [...]
     - Reason for change: [...]
     - Implementation details: [...]
   ```

Note: This prompt focuses on reconciling the gap between intended design (in manually written README files and llm.yaml) and actual implementation (reflected in .docs). It does not deal with AI-generated documentation in docs/ai-generated/, as those are derived from the codebase and should be regenerated after any implementation changes. 