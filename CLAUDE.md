# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

This is a `.github` repository, which is a special GitHub repository that provides organization-wide (or user-wide) default configurations. Files placed here apply to all repositories in the `manuelmottaherrera` account that don't have their own versions.

**IMPORTANT**: This repository MUST be:
- Named exactly `.github`
- Set as **PUBLIC** visibility (GitHub doesn't apply templates from private repos)
- Templates must be in `.github/ISSUE_TEMPLATE/` directory

## Repository Structure

```
.github/
├── .github/
│   └── ISSUE_TEMPLATE/         # Issue templates for all account repositories
│       ├── bug_report.md       # Bug report template (Spanish)
│       ├── feature_request.md  # Feature request template (Spanish)
│       ├── documentation.md    # Documentation template (Spanish)
│       └── question.md         # Question template (Spanish)
└── CLAUDE.md                   # This file
```

## Supported Organization-Wide Features

This repository can contain:

- **Issue Templates** (`.github/ISSUE_TEMPLATE/` - MUST be in this exact path)
  - Bug reports, feature requests, documentation, questions
  - Currently: 4 Spanish templates (bug, feature, docs, question)

- **Pull Request Templates** (`.github/pull_request_template.md`)
  - Default PR template for all repositories

- **Workflow Templates** (`.github/workflow-templates/`)
  - Reusable GitHub Actions workflows with metadata

- **Community Health Files**
  - `CODE_OF_CONDUCT.md` - Code of conduct
  - `CONTRIBUTING.md` - Contribution guidelines
  - `SECURITY.md` - Security policy
  - `SUPPORT.md` - Support resources
  - `FUNDING.yml` - Funding/sponsorship info

- **Profile README** (`profile/README.md`)
  - Organization profile page content

## Language and Localization

Templates in this repository are written in Spanish, reflecting the primary language for the organization's projects.

## Development Workflow

### Adding New Templates

1. Issue templates go in `.github/ISSUE_TEMPLATE/` directory (exact path required)
2. PR templates go in `.github/pull_request_template.md` or `.github/PULL_REQUEST_TEMPLATE/`
3. Workflow templates go in `.github/workflow-templates/` with corresponding `.properties.json` files

### Testing Changes

Changes to this repository take effect immediately for all organization repositories that don't override them. Test by:
1. Creating a new test repository in the organization
2. Opening an issue or PR to verify templates appear correctly
3. Delete test repository after verification

### File Naming Conventions

- Issue templates: Use kebab-case (e.g., `bug-report.md`, `feature-request.md`)
- Include YAML frontmatter for template metadata (name, about, title, labels, assignees)
- Workflow templates: Use `.yml` extension with matching `.properties.json` for metadata

## Current Configuration

The repository currently provides:
- Bug report template (`.github/ISSUE_TEMPLATE/bug_report.md`) with Spanish labels and fields
- Feature request template (`.github/ISSUE_TEMPLATE/feature_request.md`)
- Documentation template (`.github/ISSUE_TEMPLATE/documentation.md`)
- Question template (`.github/ISSUE_TEMPLATE/question.md`)
- Default assignee: `manuelmottaherrera`
- Labels automatically applied based on template type
