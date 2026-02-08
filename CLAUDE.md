# CLAUDE.md — Backend

This file provides guidance for AI assistants (including Claude Code) working in this repository.

## Repository Status

This is a newly initialized Backend repository. It does not yet contain application source code, configuration, or dependencies. The sections below should be updated as the project takes shape.

## Project Overview

- **Repository**: soju1jan/Backend
- **Purpose**: Backend service (specifics TBD — update this once the tech stack and domain are established)

## Development Workflow

### Getting Started

1. Clone the repository and check out your working branch.
2. Install dependencies once a package manager and manifest file are in place.
3. Follow the conventions listed below when adding code.

### Branch Conventions

- Feature branches use the pattern `claude/<description>-<session-id>` for AI-assisted work.
- Always push with `git push -u origin <branch-name>`.
- Write clear, descriptive commit messages. Prefer imperative mood (e.g., "Add user auth endpoint").

## Architecture & Structure

> Update this section as directories and modules are added.

Recommended layout for a typical backend project:

```
/
├── src/               # Application source code
│   ├── controllers/   # Request handlers / route controllers
│   ├── models/        # Data models / ORM entities
│   ├── routes/        # Route definitions
│   ├── middleware/     # Express/Koa/etc. middleware
│   ├── services/      # Business logic layer
│   ├── utils/         # Shared utility functions
│   └── config/        # App configuration
├── tests/             # Test files
├── migrations/        # Database migrations
├── scripts/           # Build, seed, and maintenance scripts
├── .env.example       # Environment variable template
├── package.json       # Dependencies and scripts
├── tsconfig.json      # TypeScript configuration (if applicable)
├── Dockerfile         # Container definition (if applicable)
└── CLAUDE.md          # This file
```

## Key Commands

> Populate these once the project tooling is configured.

| Task | Command |
|------|---------|
| Install dependencies | `npm install` (or equivalent) |
| Run dev server | TBD |
| Run tests | TBD |
| Lint | TBD |
| Build | TBD |
| Database migrations | TBD |

## Coding Conventions

- Keep functions small and focused.
- Prefer explicit error handling over silent failures.
- Validate all external input at system boundaries (API routes, message handlers).
- Do not commit secrets or credentials. Use environment variables and `.env` files (which should be git-ignored).
- Write tests for new functionality. Maintain existing test coverage.

## AI Assistant Guidelines

When working in this repository:

1. **Read before writing.** Always read a file before proposing changes to it.
2. **Minimal changes.** Only modify what is necessary to accomplish the task. Avoid unrelated refactors, extra comments, or speculative features.
3. **Security first.** Never introduce command injection, SQL injection, XSS, or other OWASP Top 10 vulnerabilities.
4. **No secrets in code.** Never commit `.env` files, API keys, tokens, or credentials.
5. **Test your changes.** Run the test suite after making changes. If tests fail, fix them before committing.
6. **Update this file.** When you add major infrastructure (new frameworks, databases, CI pipelines), update the relevant sections of this CLAUDE.md so future sessions have accurate context.
