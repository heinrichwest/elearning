# Claude Code Agents - Team Quick Start Guide

## What Are These Agents?

Agents are specialized AI assistants that help with specific tasks like:
- Analyzing requirements
- Generating code
- Creating documentation
- Reviewing code
- Testing features

## How to Use Agents (Super Simple)

1. Type `/` in Claude Code chat
2. Start typing the agent name (e.g., `/phase-01`)
3. Pick the agent from the list
4. The agent activates and helps you with that specific task

**Example:**
- Type `/phase-01-requirements:requirements-analysis-agent`
- Agent loads and asks what you need help with
- Tell it what you want (e.g., "Analyze the requirements for the Recruitment module")
- It does the work for you

## Setup for New Team Members (5 Minutes)

### Step 1: Get the Project
```bash
git pull
```
The `.claude` folder with all agents is already in the project.

### Step 2: Restart VSCode
- Close VSCode completely
- Reopen it
- The slash commands should now work

### Step 3: Test It
- Type `/phase-01` in Claude Code chat
- You should see available agents
- Pick one and try it

**That's it!** You're ready to use agents.

## Where Are the Agents?

All agents are stored in:
```
.claude/commands/
├── phase-01-requirements/
├── phase-02-user-design/
├── phase-03-design-system/
├── phase-04-database-architecture/
├── phase-05-api-design/
├── phase-06-database-implementation/
├── phase-07-backend-development/
├── phase-08-frontend-development/
├── phase-09-code-review-qa/
├── phase-10-testing/
├── phase-11-documentation/
├── phase-12-deployment/
├── phase-13-monitoring-maintenance/
└── phase-14-mobile-deployment/
```

## Available Agents by Phase

### Phase 1 - Requirements & Planning
- `/phase-01-requirements:requirements-analysis-agent` - Analyze requirements
- `/phase-01-requirements:technical-feasibility-agent` - Check if feature is technically possible

### Phase 2 - User Design
- `/phase-02-user-design:html-prototype-generator-agent` - Create HTML prototypes
- `/phase-02-user-design:accessibility-checker-agent` - Check accessibility
- `/phase-02-user-design:ux-review-agent` - Review user experience
- `/phase-02-user-design:test-data-generator-agent` - Generate test data

### Phase 3 - Design System
- `/phase-03-design-system:storybook-generator-agent` - Generate Storybook components
- `/phase-03-design-system:typescript-interface-generator-agent` - Generate TypeScript interfaces

### Phase 4 - Database Architecture
- `/phase-04-database-architecture:database-schema-generator-agent` - Generate database schemas
- `/phase-04-database-architecture:erd-diagram-generator-agent` - Generate ERD diagrams
- `/phase-04-database-architecture:sql-optimization-agent` - Optimize SQL queries

### Phase 5 - API Design
- `/phase-05-api-design:api-documentation-generator-agent` - Generate API docs
- `/phase-05-api-design:openapi-spec-generator-agent` - Generate OpenAPI specs

### Phase 6 - Database Implementation
- `/phase-06-database-implementation:database-performance-validator-agent` - Validate performance
- `/phase-06-database-implementation:seed-data-generator-agent` - Generate seed data

### Phase 7 - Backend Development
- `/phase-07-backend-development:code-review-agent` - Review backend code
- `/phase-07-backend-development:security-vulnerability-scanner-agent` - Scan for security issues
- `/phase-07-backend-development:unit-test-generator-agent` - Generate unit tests

### Phase 8 - Frontend Development
- `/phase-08-frontend-development:form-validation-generator-agent` - Generate form validation
- `/phase-08-frontend-development:react-hooks-generator-agent` - Generate React hooks

### Phase 9 - Code Review & QA
- `/phase-09-code-review-qa:automated-code-review-agent` - Automated code review
- `/phase-09-code-review-qa:performance-analysis-agent` - Analyze performance
- `/phase-09-code-review-qa:security-scan-agent-owasp` - OWASP security scan

### Phase 10 - Testing
- `/phase-10-testing:e2e-test-generator-agent` - Generate E2E tests
- `/phase-10-testing:visual-regression-testing-agent` - Visual regression testing
- `/phase-10-testing:test-data-generator-agent` - Generate test data

### Phase 11 - Documentation
- `/phase-11-documentation:code-documentation-generator-agent` - Generate code docs
- `/phase-11-documentation:onboarding-documentation-generator-agent` - Generate onboarding docs
- `/phase-11-documentation:user-guide-generator-agent` - Generate user guides

### Phase 12 - Deployment
- `/phase-12-deployment:deployment-verification-agent` - Verify deployments
- `/phase-12-deployment:infrastructure-as-code-generator-agent` - Generate IaC

### Phase 13 - Monitoring & Maintenance
- `/phase-13-monitoring-maintenance:log-analysis-agent` - Analyze logs
- `/phase-13-monitoring-maintenance:performance-optimization-agent` - Optimize performance

### Phase 14 - Mobile Deployment
- `/phase-14-mobile-deployment:android-play-store-deployment-agent` - Deploy to Play Store
- `/phase-14-mobile-deployment:apple-app-store-deployment-agent` - Deploy to App Store
- `/phase-14-mobile-deployment:app-store-optimization-agent` - Optimize app store presence
- `/phase-14-mobile-deployment:mobile-app-store-testing-agent` - Test mobile deployments

## How to Create a New Agent (For Team Leads)

### Quick Version:
1. Create a `.md` file in the appropriate phase folder
2. Add the agent instructions
3. Commit and push
4. Team members pull and restart VSCode

### Detailed Example:

**Step 1: Create the file**
```
.claude/commands/phase-05-api-design/my-new-agent.md
```

**Step 2: Write the agent prompt**
```markdown
# My New Agent

You are specialized in [what this agent does].

## Your Role
[Explain what the agent should do]

## Key Responsibilities
1. [Responsibility 1]
2. [Responsibility 2]
3. [Responsibility 3]

## Tools You Should Use
- **Read**: To read files
- **Write**: To create files
- **Bash**: To run commands
- **Grep**: To search code

## Best Practices
1. [Practice 1]
2. [Practice 2]

## Model Configuration
Use **claude-sonnet-4-5** for complex tasks.
Use **claude-haiku-3-5** for simple tasks.
```

**Step 3: Save, commit, push**
```bash
git add .claude/commands/phase-05-api-design/my-new-agent.md
git commit -m "Add new API design agent"
git push
```

**Step 4: Team uses it**
- Team members pull the changes
- Restart VSCode
- Use `/phase-05-api-design:my-new-agent`

## Important Rules for Folder Structure

### ✅ DO THIS:
- Keep agents in phase folders
- Use lowercase folder names
- Use hyphens instead of spaces (e.g., `phase-01-requirements`)
- Name agent files descriptively (e.g., `requirements-analysis-agent.md`)

### ❌ DON'T DO THIS:
- Don't use spaces in folder names (e.g., ~~`Phase 1 - Requirements`~~)
- Don't use special characters like `&` in folder names
- Don't put agents directly in `.claude/commands/` root (keeps it clean)
- Don't create wrapper files (not needed with simple folder names)

## Troubleshooting

### Problem: Slash commands not showing up

**Solution:**
1. Make sure you pulled the latest code: `git pull`
2. Restart VSCode completely (close and reopen)
3. Type `/` and wait a second for the list to load

### Problem: Agent shows "wibbling" but doesn't run

**Solution:**
1. Check that folder names have no spaces
2. Folder names should be lowercase with hyphens (e.g., `phase-01-requirements`)
3. Restart VSCode after fixing folder names

### Problem: Can't find a specific agent

**Solution:**
1. Type `/phase-` and browse the list
2. Check this guide for the exact command name
3. Check if the agent file exists in the `.claude/commands/` folder

## Tips for Using Agents Effectively

1. **Be specific**: Tell the agent exactly what you need
   - ❌ "Help me with code"
   - ✅ "Generate unit tests for the QualificationService.cs class"

2. **Provide context**: Reference specific files or features
   - ❌ "Review my code"
   - ✅ "Review the RecruitmentController.cs for security vulnerabilities"

3. **Use the right agent**: Pick the phase that matches your task
   - Writing API code? → Use Phase 7 (Backend Development)
   - Creating tests? → Use Phase 10 (Testing)
   - Writing docs? → Use Phase 11 (Documentation)

4. **Ask follow-up questions**: Agents can clarify and iterate
   - If the agent's output isn't what you need, ask it to adjust

## Questions?

- Check the main README.md for more details
- Ask your team lead
- Check Claude Code docs: https://docs.claude.com/claude-code

---

**Remember:** The `.claude` folder is part of the project. When you pull code, you get all agents automatically. Just restart VSCode and start using them!
