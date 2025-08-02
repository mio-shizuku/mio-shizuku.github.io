# Official Website

[![CI](https://github.com/mio-shizuku/official-website/actions/workflows/ci.yml/badge.svg)](https://github.com/mio-shizuku/official-website/actions/workflows/ci.yml)
[![Dependabot Updates](https://github.com/mio-shizuku/official-website/actions/workflows/dependabot/dependabot-updates/badge.svg)](https://github.com/mio-shizuku/official-website/actions/workflows/dependabot/dependabot-updates)
[![CodeQL](https://github.com/mio-shizuku/official-website/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/mio-shizuku/official-website/actions/workflows/github-code-scanning/codeql)
[![License](https://img.shields.io/badge/license-MIT-blue)](#license)
[![Hugo](https://img.shields.io/badge/Hugo-v0.148-orange)](https://gohugo.io/)

Organization official website built with [Hugo](https://gohugo.io/) and [Hextra](https://imfing.github.io/hextra/) theme.

## Live Site

- [mio-shizuku.shettydev.com](https://mio-shizuku.shettydev.com/)

## Locally Preview

### Prerequisites

- [Hugo Extended](https://gohugo.io/installation/) (v0.148.2 or later)
- [Go](https://golang.org/doc/install) (v1.24.5 or later)

### Steps

#### Using Makefile (Recommended)

```bash
# Preview the site locally (with drafts)
make preview

# Build the site for production
make build

# Clean build artifacts
make clean

# Show available commands
make help
```

#### Using Hugo Commands Directly

```bash
# Start development server
hugo server -D

# Build for production
hugo --gc --minify
```

## License

### Code

The source code of this website is licensed under the [MIT License](LICENSE).

### Content

The documentation and content (including blog posts, articles, and other written materials) are licensed under the [Creative Commons Attribution 4.0 International License (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).

This means:

- **Code**: You can freely use, modify, and distribute the code
- **Content**: You can share and adapt the content, as long as you provide appropriate attribution

For more details, see the [LICENSE](LICENSE) file for code licensing terms.
