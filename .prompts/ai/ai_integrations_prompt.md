Document external interactions and extension points:
1. External APIs/services (protocols, formats, auth)
2. Extension frameworks or plugin points
3. Optional frontend analysis if applicable (UI framework, key patterns)
4. Model-specific implementation details:
   - Provider-specific optimizations
   - Resource management patterns
5. Note cross-cutting integrations or extension points used by multiple modules.
6. Mention relevant `.docs` files that might clarify how these APIs fit into the overall system (such as "architecture_context.md").

ACCURACY REQUIREMENTS:
- Document ONLY APIs and integrations with concrete implementation in the code
- Include file references (filename:line) for each API usage or integration point
- Base all protocol/format information on actual API calls in the codebase
- Mark any API or integration that lacks clear implementation as "Referenced but not implemented"
- DO NOT speculate about the purpose of APIs beyond what is evident in the code

Keep it concise for LLM consumption.
Save as "integrations_context.md" in ".docs". 