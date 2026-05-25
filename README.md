# Oshorial Lore Wiki

This repository contains the source for the Oshorial campaign wiki, built with Jekyll and deployed with GitHub Pages.

## What You Need

- Ruby (recommended: latest stable)
- Bundler (`gem install bundler`)
- A terminal on macOS or Windows

## Run Locally on macOS

1. Open Terminal and change into the repository:

```bash
cd /Users/patrickfaulkner/Documents/repos/oshorial-lore-wiki
```

2. Install dependencies:

```bash
bundle install
```

3. Start the local site server:

```bash
bundle exec jekyll serve --livereload
```

4. Open the site in your browser at:

```text
http://127.0.0.1:4000
```

## Run Locally on Windows

1. Open PowerShell or Windows Terminal and change into the repository:

```powershell
cd C:\Users\<your-username>\Documents\repos\oshorial-lore-wiki
```

2. Install dependencies:

```powershell
bundle install
```

3. Start the local site server:

```powershell
bundle exec jekyll serve --livereload
```

4. Open the site in your browser at:

```text
http://127.0.0.1:4000
```

## Useful Commands

Build the static site without serving it locally:

```bash
bundle exec jekyll build
```

## Content Layout

- `docs/index.html` - Home page
- `docs/locations/` - Location pages
- `docs/npcs/` - NPC pages
- `docs/players/` - Player character pages
- `docs/_layouts/default.html` - Shared Jekyll page layout

## Notes

- This repository uses `docs/` as the Jekyll source directory.
- Add new content as `.html` files with Jekyll front matter (`---` block at the top).