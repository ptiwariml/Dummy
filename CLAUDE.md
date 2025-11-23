# CLAUDE.md - AI Assistant Guide for Dummy Repository

**Last Updated:** 2025-11-23
**Repository:** ptiwariml/Dummy
**Purpose:** Test/demonstration repository

---

## Table of Contents

1. [Repository Overview](#repository-overview)
2. [Codebase Structure](#codebase-structure)
3. [Development Workflows](#development-workflows)
4. [Git Conventions](#git-conventions)
5. [Key Conventions for AI Assistants](#key-conventions-for-ai-assistants)
6. [Common Tasks](#common-tasks)

---

## Repository Overview

### Purpose
This is a minimal test/demonstration repository used for prototyping, testing, and educational purposes.

### Current State
- **Primary Files:** README.md
- **Language/Framework:** None (minimal repository)
- **Dependencies:** None
- **Build System:** None
- **Testing Framework:** None

### Repository Metadata
- **Owner:** ptiwariml
- **Repository Name:** Dummy
- **Remote URL:** http://local_proxy@127.0.0.1:55531/git/ptiwariml/Dummy

---

## Codebase Structure

```
Dummy/
├── .git/               # Git repository metadata
│   ├── hooks/         # Git hooks (sample only)
│   └── ...
├── README.md          # Basic repository documentation
└── CLAUDE.md          # This file - AI assistant guidelines
```

### Key Files

- **README.md** - Minimal documentation (currently empty)
- **CLAUDE.md** - AI assistant guidelines and repository context

---

## Development Workflows

### Working with this Repository

Since this is a test/demonstration repository:

1. **Experimentation Friendly:** This repository is designed for testing and experimentation
2. **No Critical Dependencies:** Changes here won't affect production systems
3. **Flexible Structure:** Feel free to add files, directories, or configurations as needed
4. **Documentation First:** Always update this CLAUDE.md when making structural changes

### Adding New Features

When adding new functionality:

1. **Create appropriate directory structure** if needed (e.g., `src/`, `tests/`, `docs/`)
2. **Update README.md** with relevant information
3. **Update this CLAUDE.md** to reflect new structure and conventions
4. **Use appropriate git branching** (see Git Conventions below)

---

## Git Conventions

### Branch Naming

**CRITICAL:** This repository uses a special branch naming convention for AI assistant work:

- **Pattern:** `claude/claude-md-mibb4b8fed5zlucb-01Szhgsr7fsRYcmYvNBg4vkX`
- **Format:** `claude/` prefix + session-specific identifier
- **Current Branch:** `claude/claude-md-mibb4b8fed5zlucb-01Szhgsr7fsRYcmYvNBg4vkX`

### Important Git Rules

1. **Branch Naming:**
   - All AI assistant branches MUST start with `claude/`
   - Branch name must match the session ID provided in task context
   - Pushing to incorrectly named branches will fail with HTTP 403

2. **Push Operations:**
   ```bash
   # Always use -u flag for first push
   git push -u origin <branch-name>

   # Retry logic for network errors (up to 4 times)
   # Wait times: 2s, 4s, 8s, 16s between retries
   ```

3. **Fetch/Pull Operations:**
   ```bash
   # Prefer specific branch fetches
   git fetch origin <branch-name>

   # For pulls
   git pull origin <branch-name>
   ```

4. **Commit Messages:**
   - Use clear, descriptive commit messages
   - Focus on the "why" rather than just the "what"
   - Examples:
     - ✅ "Add CLAUDE.md to document repository structure for AI assistants"
     - ❌ "Update files"

### Commit History

Current commit history (most recent first):
```
ac1e836 - Update README.md
da30e8a - Update README.md
15e1a09 - Initial commit
```

---

## Key Conventions for AI Assistants

### General Guidelines

1. **Read Before Writing:**
   - Always read existing files before modifying them
   - Understand the current state before making changes
   - Never propose changes to code you haven't examined

2. **Minimal Changes:**
   - Only make changes that are directly requested
   - Avoid over-engineering or adding unnecessary features
   - Don't add improvements that weren't asked for

3. **Documentation:**
   - Update README.md when adding user-facing features
   - Update CLAUDE.md when changing repository structure or workflows
   - Keep documentation concise and relevant

4. **File Operations:**
   - Prefer editing existing files over creating new ones
   - Only create new files when absolutely necessary
   - Use appropriate tools: Read, Edit, Write (not bash commands)

### Security Considerations

- No sensitive data currently stored in this repository
- If adding configuration files, never commit secrets or credentials
- Use environment variables or .env files (added to .gitignore) for sensitive data

### Code Style

Since this is a minimal repository with no specific language:
- Follow language-specific best practices when code is added
- Maintain consistency with existing code style
- Use appropriate linting/formatting tools when available

---

## Common Tasks

### Task: Add New Content

1. Determine appropriate location for new files
2. Create necessary directory structure
3. Add files using Write tool
4. Update documentation (README.md and CLAUDE.md)
5. Commit with descriptive message
6. Push to correct branch

### Task: Modify Existing Files

1. Read current file contents
2. Use Edit tool for modifications
3. Verify changes are minimal and focused
4. Commit with clear message explaining the change
5. Push to correct branch

### Task: Repository Analysis

1. Use Glob to find all files
2. Read key files (README, configuration files, source files)
3. Analyze structure and patterns
4. Document findings in response or update CLAUDE.md

### Task: Create Pull Request

1. Ensure all changes are committed
2. Push to feature branch (claude/* branch)
3. Use `gh pr create` with:
   - Clear title describing the changes
   - Summary section with bullet points
   - Test plan with verification steps

---

## Extension Points

As this repository grows, consider adding:

- **Programming Language Specifics:** Code style guides, linting rules
- **Build Configuration:** Package management, build scripts, CI/CD
- **Testing Guidelines:** Test frameworks, coverage requirements, testing patterns
- **Deployment Procedures:** If applicable
- **Architecture Documentation:** System design, component relationships
- **API Documentation:** If APIs are developed
- **Troubleshooting Guide:** Common issues and solutions

---

## Notes for Future AI Assistants

### Repository Evolution

This repository is currently minimal but may evolve into:
- A code playground/sandbox
- A testing ground for new technologies
- A demonstration/tutorial repository
- A prototype for larger projects

### Maintaining This Document

When updating CLAUDE.md:
1. Update the "Last Updated" date at the top
2. Add new sections as the repository grows
3. Archive obsolete information rather than deleting it
4. Keep the Table of Contents synchronized
5. Maintain clear, concise language

### Getting Help

- Check README.md for user-facing documentation
- Review recent commit history for context
- Analyze existing code before asking questions
- Use search tools (Grep, Glob) to understand patterns

---

## Metadata

**Document Version:** 1.0
**Created:** 2025-11-23
**Template Basis:** Minimal repository analysis
**Applicable Sessions:** All AI assistant sessions working with this repository
