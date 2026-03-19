# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Purpose

LeetCode training repository with solutions in Python, Java, and TypeScript/JavaScript.

## Learning Mode

When helping with problems, default to **guiding** rather than giving full solutions:
- Ask what approach the user is considering first
- Give hints and nudges toward the right algorithm/data structure
- Only provide full solutions when explicitly asked
- After solving, discuss time/space complexity and alternative approaches

## Languages and Testing

### Python
```bash
python3 solution.py          # run directly
python3 -m pytest solution.py  # if test functions included
```

### Java
```bash
javac Solution.java && java Solution
```

### TypeScript/JavaScript
```bash
npx ts-node solution.ts    # TypeScript
node solution.js            # JavaScript
```

## Obsidian Integration

Notes for solved problems go in the Obsidian vault at `Codes/Backend/Algorithm/`. Use the Obsidian MCP tools to read/write notes.

**Note format** (match existing style):
- No frontmatter
- Code blocks first with inline comments explaining the "why"
- Extract general patterns at the end (e.g., "early exit on failure" pattern)
- Use analogies and memorable explanations in comments
- Detailed breakdowns of key language-specific methods/concepts used

After solving a problem, offer to create/update an Obsidian note capturing the solution, key insights, and reusable patterns.

## Neovim Integration

User runs Neovim with a kickstart-based LazyVim config at `~/.config/nvim/`. LSP is configured via Mason for Python (pylsp + ruff), TypeScript (ts_ls), and Java (jdtls).
