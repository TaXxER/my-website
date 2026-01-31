# Niek Tax - Personal Website (Hugo Blox)

This website is built using [Hugo](https://gohugo.io/) and the [Hugo Blox Builder](https://hugoblox.com/) (formerly Hugo Academic).

## Prerequisites

You need to have **Hugo** (Extended version) and **Go** installed on your system.

### macOS (Homebrew)
```bash
brew install hugo go
```

## Setup

1. Initialize the Go module:
   ```bash
   hugo mod init my-website
   ```

2. Update dependencies:
   ```bash
   hugo mod get -u
   hugo mod tidy
   ```

## Running Locally

To start the local development server:

```bash
hugo server
```

Navigate to `http://localhost:1313/` in your browser.

## Content Management

- **Profile**: Edit `content/authors/admin/_index.md`
- **Homepage Widgets**: Edit files in `content/home/`
- **Publications**: Add BibTeX files or manually add markdown files in `content/publication/` (create folder if needed)

## Deployment to GitHub Pages

1. Build the site:
   ```bash
   hugo
   ```
   This generates the static site in the `public/` directory.

2. Push the contents of `public/` to your GitHub repository (or configure a GitHub Action to build automatically).
