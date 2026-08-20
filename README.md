# AI Code Reviewer

![CI](https://github.com/Qyroxen/AI-Code-Reviewer/actions/workflows/ci.yml/badge.svg) ![Go](https://img.shields.io/badge/Go-1.23+-00ADD8?style=flat&logo=go) ![License](https://img.shields.io/badge/License-MIT-yellow.svg) ![Stars](https://img.shields.io/github/stars/Qyroxen/AI-Code-Reviewer?style=social)

> AI-powered code review that catches bugs before your users do

[![Star Badge](https://img.shields.io/github/stars/Qyroxen/AI-Code-Reviewer?style=social)](https://github.com/Qyroxen/AI-Code-Reviewer/stargazers)

## What is it?

AI Code Reviewer uses local LLM to analyze your code for bugs, security issues, and code smells. Runs offline, keeps your code private.

## Why should you care?

Manual code reviews are slow and miss things. AI Code Reviewer catches 80% of issues in seconds.

## Demo

```bash
./ai-code-reviewer review --path ./my-project
```

**Output:**
```
Found 3 issues:
  HIGH: SQL Injection in db.go:42
  MEDIUM: Unused variable in main.go:15
  LOW: Missing error handling in utils.go:8
```

## Features

- AI-powered analysis using Ollama (local LLM)
- Detects: SQL injection, XSS, hardcoded secrets, code smells
- Severity levels: Critical, High, Medium, Low
- JSON export for CI/CD integration
- 100% offline - your code never leaves your machine

## Quick Start

```bash
# Install
git clone https://github.com/Qyroxen/AI-Code-Reviewer.git
cd AI-Code-Reviewer
go build -o ai-code-reviewer .

# Run
./ai-code-reviewer --path ./my-project
```

## CLI Flags

| Flag | Description | Default |
|------|-------------|---------|
| `--path` | Target directory | `.` |
| `--model` | LLM model to use | `llama3` |
| `--format` | Output format (text, json) | `text` |
| `--severity` | Minimum severity level | `low` |
| `--fix` | Auto-fix issues | `false` |

## Examples

# Basic review
./ai-code-reviewer review --path ./src

# With auto-fix
./ai-code-reviewer review --path ./src --fix

# JSON output for CI
./ai-code-reviewer review --path ./src --format json > report.json

# High severity only
./ai-code-reviewer review --path ./src --severity high

## Contributing

Contributions are welcome! Please see [CONTRIBUTING.md](CONTRIBUTING.md) for details.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

<p align="center">
  <a href="https://github.com/Qyroxen/AI-Code-Reviewer/stargazers">
    <img src="https://img.shields.io/github/stars/Qyroxen/AI-Code-Reviewer?style=social" alt="Star this repo">
  </a>
  <a href="https://github.com/Qyroxen/AI-Code-Reviewer/network/members">
    <img src="https://img.shields.io/github/forks/Qyroxen/AI-Code-Reviewer?style=social" alt="Fork this repo">
  </a>
  <a href="https://github.com/Qyroxen/AI-Code-Reviewer/issues">
    <img src="https://img.shields.io/github/issues/Qyroxen/AI-Code-Reviewer" alt="Issues">
  </a>
</p>
