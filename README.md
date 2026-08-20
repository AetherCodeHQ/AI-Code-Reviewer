# AI Code Reviewer

![CI](https://github.com/Qyroxen/AI-Code-Reviewer/actions/workflows/ci.yml/badge.svg)
![CodeQL](https://github.com/Qyroxen/AI-Code-Reviewer/actions/workflows/codeql.yml/badge.svg)
![Go](https://img.shields.io/badge/Go-1.23+-00ADD8?style=flat&logo=go)
![License](https://img.shields.io/badge/License-MIT-yellow.svg)
![Stars](https://img.shields.io/github/stars/Qyroxen/AI-Code-Reviewer?style=social)
![Issues](https://img.shields.io/github/issues/Qyroxen/AI-Code-Reviewer)
![PRs](https://img.shields.io/github/issues-pr/Qyroxen/AI-Code-Reviewer)

> A production-ready CLI tool built with Go

[![Star Badge](https://img.shields.io/github/stars/Qyroxen/AI-Code-Reviewer?style=social)](https://github.com/Qyroxen/AI-Code-Reviewer/stargazers)

## What is it?

AI Code Reviewer is a production-ready CLI tool built with Go. It provides powerful functionality with a beautiful terminal interface.

## Features

- Fast and efficient (written in Go)
- Beautiful CLI with colored output
- Comprehensive documentation
- GitHub Actions CI/CD
- CodeQL security analysis
- Dependabot for dependency updates
- MIT Licensed
- Fully offline - zero cloud dependency

## Quick Start

```bash
# Install
git clone https://github.com/Qyroxen/AI-Code-Reviewer.git
cd AI-Code-Reviewer
go build -o aicodereviewer .

# Run
./aicodereviewer --help
```

## CLI Usage

```bash
# Basic usage
./aicodereviewer

# With flags
./aicodereviewer --verbose --output json

# Get help
./aicodereviewer --help
```

## Examples

```bash
# Example 1
./aicodereviewer example1

# Example 2
./aicodereviewer example2 --flag value
```

## Development

```bash
# Run tests
go test ./...

# Build
go build -o aicodereviewer .

# Lint
golangci-lint run

# Security scan
codeql analyze
```

## Contributing

Contributions are welcome! Please see [CONTRIBUTING.md](CONTRIBUTING.md) for details.

## Security

For security vulnerabilities, please see [SECURITY.md](SECURITY.md).

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

<p align="center">
  <a href="https://github.com/Qyroxen/AI-Code-Reviewer/stargazers">
    <img src="https://img.shields.io/github/stars/Qyroxen/AI-Code-Reviewer?style=social" alt="Star this repo">
  </a>
  <a href="https://github.com/Qyroxen/AI-Code-Reviewer/forks">
    <img src="https://img.shields.io/github/forks/Qyroxen/AI-Code-Reviewer?style=social" alt="Fork this repo">
  </a>
  <a href="https://github.com/Qyroxen/AI-Code-Reviewer/issues">
    <img src="https://img.shields.io/github/issues/Qyroxen/AI-Code-Reviewer" alt="Issues">
  </a>
  <a href="https://github.com/Qyroxen/AI-Code-Reviewer/pulls">
    <img src="https://img.shields.io/github/issues-pr/Qyroxen/AI-Code-Reviewer" alt="Pull Requests">
  </a>
</p>
