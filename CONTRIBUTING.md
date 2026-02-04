# Contributing to Tribo Skills

Thank you for your interest in contributing to Tribo Skills! This marketplace contains 84 marketing skills for Claude Code, and we welcome contributions that improve existing skills or add new ones.

## Table of Contents

- [Getting Started](#getting-started)
- [Adding a New Skill](#adding-a-new-skill)
- [Improving Existing Skills](#improving-existing-skills)
- [Pull Request Process](#pull-request-process)
- [Quality Standards](#quality-standards)
- [Code of Conduct](#code-of-conduct)

## Getting Started

1. Fork the repository
2. Clone your fork locally:
   ```bash
   git clone https://github.com/your-username/tribo-skills.git
   cd tribo-skills
   ```
3. Create a branch for your changes:
   ```bash
   git checkout -b add-new-skill
   ```

## Adding a New Skill

### Directory Structure

Each skill is a plugin with this structure:

```
plugins/
└── your-skill-name/           # kebab-case name
    ├── .claude-plugin/
    │   └── plugin.json        # Plugin manifest
    ├── skills/
    │   └── your-skill-name/
    │       └── SKILL.md       # Skill definition
    └── README.md              # Optional documentation
```

### Step 1: Create the Plugin Directory

```bash
mkdir -p plugins/your-skill-name/.claude-plugin
mkdir -p plugins/your-skill-name/skills/your-skill-name
```

### Step 2: Create plugin.json

Create `plugins/your-skill-name/.claude-plugin/plugin.json`:

```json
{
  "name": "your-skill-name",
  "description": "A brief description of what this skill does (1-2 sentences)",
  "version": "1.0.0",
  "author": {
    "name": "Your Name"
  },
  "license": "MIT",
  "keywords": ["marketing", "your-skill-name", "relevant", "keywords"]
}
```

### Step 3: Create SKILL.md

Create `plugins/your-skill-name/skills/your-skill-name/SKILL.md`:

```markdown
---
name: your-skill-name
description: A comprehensive description of what this skill does, who should use it, and when to use it. Include key methodologies, frameworks, or experts referenced.
---

# Skill Title

## Overview
Brief introduction to the skill and its purpose.

## Discovery & Planning Questions
Questions Claude should ask the user before starting work:
1. Question about target audience
2. Question about goals
3. Question about constraints

## Core Frameworks

### Framework 1
Explanation of the first framework or methodology.

### Framework 2
Explanation of the second framework or methodology.

## Execution Process

### Step 1: Research
How to approach research.

### Step 2: Strategy
How to develop strategy.

### Step 3: Implementation
How to execute.

## Output Templates

### Template 1
Example output format.

## Quality Checklist
- [ ] Checkpoint 1
- [ ] Checkpoint 2
- [ ] Checkpoint 3

## References
- Book/Resource 1
- Book/Resource 2
```

### Step 4: Add to Marketplace

Add your skill to `.claude-plugin/marketplace.json`:

```json
{
  "name": "your-skill-name",
  "source": "your-skill-name",
  "description": "Same description as plugin.json",
  "version": "1.0.0",
  "author": { "name": "Your Name" },
  "license": "MIT",
  "keywords": ["marketing", "your-skill-name"]
}
```

### Step 5: Test Locally

```bash
# Add the local marketplace
claude plugins marketplace add ./

# Install your skill
claude plugins install your-skill-name@tribo-skills

# Test the skill
/your-skill-name
```

## Improving Existing Skills

1. Navigate to the skill in `plugins/skill-name/skills/skill-name/SKILL.md`
2. Make your improvements
3. Update the version in both `plugin.json` and `marketplace.json`
4. Submit a pull request with clear description of changes

### What to Improve

- Add missing frameworks or methodologies
- Include better examples
- Add discovery questions
- Improve output templates
- Fix typos or unclear instructions
- Add references to source materials

## Pull Request Process

1. **Title**: Use a clear, descriptive title
   - `Add: new-skill-name` for new skills
   - `Improve: skill-name - added X framework` for improvements
   - `Fix: skill-name - typo in section Y` for fixes

2. **Description**: Include:
   - What the skill does (for new skills)
   - What you changed and why (for improvements)
   - How you tested it

3. **Checklist**:
   - [ ] Skill has valid `plugin.json`
   - [ ] SKILL.md has required frontmatter (name, description)
   - [ ] Skill is added to `marketplace.json`
   - [ ] JSON files are valid (no syntax errors)
   - [ ] Tested locally with Claude Code

4. **Review**: Wait for review. Address any feedback.

## Quality Standards

### SKILL.md Requirements

| Requirement | Description |
|-------------|-------------|
| Frontmatter | Must include `name` and `description` |
| Overview | Clear explanation of what the skill does |
| Discovery Questions | At least 3 questions to understand user needs |
| Frameworks | At least one methodology or framework |
| Examples | Practical examples or templates |

### Writing Guidelines

- **Be specific**: Include exact frameworks, not vague advice
- **Cite sources**: Reference books, experts, or methodologies
- **Be actionable**: Provide steps Claude can follow
- **Include examples**: Show expected outputs
- **Stay focused**: One skill per plugin

### Naming Conventions

- **Folder names**: `kebab-case` (e.g., `email-marketing`)
- **Skill names**: `kebab-case` matching folder name
- **Descriptions**: Start with verb (e.g., "Creates...", "Helps...")

## Code of Conduct

### Our Standards

- Be respectful and inclusive
- Provide constructive feedback
- Focus on the contribution, not the contributor
- Help newcomers learn

### Unacceptable Behavior

- Harassment or discrimination
- Trolling or personal attacks
- Publishing others' private information
- Spamming or off-topic content

### Reporting

Report issues to the repository maintainers via GitHub issues.

---

Questions? Open an issue or reach out to the maintainers.

Thank you for contributing to Tribo Skills!
