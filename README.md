# Glowyr Inc. Website

Static site built with Jekyll using the TeXt theme. Deployed to GitHub Pages via Actions (artifact publish).

## Prerequisites
- Ruby 3.1+ (3.2 used in CI) and Bundler
- macOS: use rbenv or asdf to manage Ruby, or system Ruby if suitable

## Setup
```bash
bundle config set --local path 'vendor/bundle'
bundle install
```

## Run a local server
```bash
bundle exec jekyll serve
```
- Open http://localhost:4000
- Optional: `bundle exec jekyll serve --livereload`

## Build for production
```bash
JEKYLL_ENV=production bundle exec jekyll build
```
- Output in `_site/`

## Clean build artifacts
```bash
bundle exec jekyll clean
```

## Update gems
```bash
bundle update
```

## Project structure (key files)
- `_config.yml` — site configuration and theme settings
- `_data/navigation.yml` — header navigation links
- `_includes/head/favicon.html` — favicon override (pickaxe icon)
- `assets/favicon.svg` — current favicon
- `index.html` — home page (dark header)
- `about.md`, `services.md`, `contact.md`, `404.html` — content pages
- `.github/workflows/pages.yml` — GitHub Pages deployment via Actions
- `CNAME` — custom domain (glowyr.ca)

## Deployment (GitHub Pages)
- Workflow builds on pushes to `main` and deploys a Pages artifact
- In GitHub → Settings → Pages: set Build & deployment to GitHub Actions
- DNS for glowyr.ca (apex): set A records to GitHub Pages IPs
  - 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153
- `CNAME` ensures the custom domain and HTTPS enforcement

## Editing notes
- To use a dark header on a page, add to front matter:
  ```yaml
  header:
    theme: dark
  ```
- Update navigation in `_data/navigation.yml`
- Replace favicon by swapping `assets/favicon.svg` and, if needed, updating `_includes/head/favicon.html`

## Troubleshooting
- YAML front matter must be wrapped with `---` at top of files
- If port 4000 is in use: `bundle exec jekyll serve --port 4001`
- If WEBrick is missing on Ruby 3+: it’s included in `Gemfile`
- Clear caches if odd behavior: `bundle exec jekyll clean && rm -rf .jekyll-cache`
