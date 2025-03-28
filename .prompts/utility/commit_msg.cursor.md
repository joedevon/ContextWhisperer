1. Analyze the changes in this repository since the last commit:
   - Use `git diff` to review changes
   - Group related changes by feature, fix, or logical unit
   - For each group, note:
     * What files changed
     * Which parts of each file belong to this change
     * Dependencies between changes

2. For changes that cross categories:
   - Use `git add -p` to stage specific hunks
   - Group hunks by their purpose
   - Note which parts of files go together

3. For each logical group of changes:
   - Generate a commit message following conventional commits:
     * Type: feat|fix|docs|style|refactor|test|chore
     * Format: type(scope): concise title
     * Brief bullet points for significant changes
     * Breaking changes marked with BREAKING CHANGE:

4. Propose commits in dependency order:
   ```
   1. feat(auth): implement basic login flow
      * src/auth/login.ts (functions: loginUser, validateToken)
      * src/components/LoginForm.tsx (entire file)

   2. style(ui): update button styles
      * src/components/Button.tsx (styles only)
      * src/components/LoginForm.tsx (button styling changes)
   ```

5. Execute commits:
   - For each commit:
     * Use `git add -p` if needed to stage specific changes
     * Commit with generated message
   - Push when all commits are ready