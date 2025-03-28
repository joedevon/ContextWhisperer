Summarize essential operational details:
1. Logging, secrets, and config (libraries, env usage)
2. Testing approaches (unit, integration, key frameworks)
3. Build & local dev patterns (build tools, code style)
4. Deployment & CI/CD (pipeline steps, environment handling)
5. Observability & monitoring:
   - Specific metrics being collected and granularity
   - Performance optimization patterns
   - Alerting and dashboards
6. Note any cross-cutting operational concerns that affect multiple areas (for example, logging patterns used throughout).

ACCURACY REQUIREMENTS:
- Document ONLY operational tools and patterns that have evidence in the codebase
- Include file references (filename:line) for key configurations
- Base all tooling information on package files, configs, or CI scripts
- Label any operational aspects without clear evidence as "Not found in codebase"
- DO NOT assume deployment or monitoring approaches without supporting files

Focus on minimal information an LLM can parse easily.
Save as "operations_context.md" in ".docs". 