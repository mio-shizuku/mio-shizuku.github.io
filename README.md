# Official Website

Organization official website built with [Hugo](https://gohugo.io/) and [Hextra](https://imfing.github.io/hextra/) theme.

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
