# Claude Code Guidelines for Sthandweni Repository

## Project Context
This is an Olympic weightlifting project. The repository may be accessed from multiple devices including:
- Multiple computers
- Personal laptop
- GitHub Codespaces
- Other development environments

## Critical Git Workflow Rules

### 1. Push Changes Frequently
**ALWAYS** ask the user for permission to push changes to GitHub after completing ANY significant work, including:
- Bug fixes
- Feature additions
- Code refactoring
- Configuration changes
- Documentation updates
- Even small improvements

### 2. Proactive Push Prompts
- Ask "Would you like me to push these changes to GitHub?" frequently throughout the session
- Ask immediately after the user expresses satisfaction with progress
- Ask after completing each major task or milestone
- Ask before ending a work session
- When in doubt, ask to push

### 3. Standard Git Workflow

When user approves pushing changes:

1. **Stage changes**: `git add .` (or specific files)
2. **Create commit** with descriptive message following this format:
   ```
   <type>: <description>

   - Detail 1
   - Detail 2

   🤖 Generated with [Claude Code](https://claude.com/claude-code)

   Co-Authored-By: Claude <noreply@anthropic.com>
   ```

3. **Push to remote**: `git push origin main` (or current branch)
4. **Verify**: Run `git status` to confirm clean state

### 4. Commit Message Types
- `feat`: New feature
- `fix`: Bug fix
- `refactor`: Code refactoring
- `docs`: Documentation changes
- `style`: Code formatting/style
- `test`: Adding or updating tests
- `chore`: Maintenance tasks
- `perf`: Performance improvements

### 5. Before Pushing
Always run these checks:
- `git status` - See what's changed
- `git diff` - Review the changes
- Ensure no sensitive data (API keys, passwords, etc.) are included

### 6. Multi-Device Synchronization Priority
The goal is to ensure ALL devices can access the most up-to-date code at ALL times. This means:
- Push early and push often
- Never leave uncommitted work at end of session
- Always pull before starting work: `git pull origin main`

### 7. Handling Conflicts
If push fails due to remote changes:
1. Run `git pull --rebase origin main`
2. Resolve any conflicts if they occur
3. Run `git push origin main`

## Example Workflow

```bash
# At start of session
git pull origin main

# After completing work
git status
git diff
git add .
git commit -m "$(cat <<'EOF'
feat: Add Olympic weightlifting training tracker

- Implement snatch PR tracking
- Add clean & jerk calculator
- Create workout history view

🤖 Generated with [Claude Code](https://claude.com/claude-code)

Co-Authored-By: Claude <noreply@anthropic.com>
EOF
)"
git push origin main
git status
```

## Reminders for Claude
- **ASK OFTEN**: "Would you like me to push these changes to GitHub?"
- **AFTER EVERY MILESTONE**: Prompt for push
- **USER SATISFACTION**: When user says they're happy with progress, immediately offer to push
- **SESSION END**: Always offer to push before ending work
- **SYNC IS CRITICAL**: Multi-device access depends on frequent pushing

## Olympic Weightlifting Context
This project involves Olympic weightlifting (snatch, clean & jerk, etc.). Keep this context in mind when:
- Writing commit messages
- Creating features
- Understanding user requirements
- Suggesting improvements
