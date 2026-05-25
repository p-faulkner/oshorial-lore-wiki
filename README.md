# Oshorial Lore Wiki

This repository contains the source for the Oshorial campaign wiki, built with Jekyll and deployed with GitHub Pages.

## What You Need

- Ruby 3.1.x (tested with 3.1.7)
- Bundler (`gem install bundler`)
- A terminal on macOS or Windows

## Run Locally on macOS

1. Open Terminal and change into the repository:

```bash
cd /Users/patrickfaulkner/Documents/repos/oshorial-lore-wiki
```

2. Ensure a compatible Ruby is first on your `PATH`:

```bash
export PATH="/opt/homebrew/opt/ruby@3.1/bin:$PATH"
ruby -v
```

3. Install dependencies:

```bash
gem install bundler
bundle install
```

4. Start the local site server:

```bash
bundle exec jekyll serve --livereload
```

5. Open the site in your browser at:

```text
http://127.0.0.1:4000
```

## Run Locally on Windows

1. Open PowerShell or Windows Terminal and change into the repository:

```powershell
cd C:\Users\<your-username>\Documents\repos\oshorial-lore-wiki
```

2. Confirm Ruby 3.1.x is active:

```powershell
ruby -v
```

3. Install dependencies:

```powershell
gem install bundler
bundle install
```

4. Start the local site server:

```powershell
bundle exec jekyll serve --livereload
```

5. Open the site in your browser at:

```text
http://127.0.0.1:4000
```

## Make Ruby 3.1 Default (macOS)

Add this to your shell profile so new terminals use Ruby 3.1 automatically:

```bash
echo 'export PATH="/opt/homebrew/opt/ruby@3.1/bin:$PATH"' >> ~/.zshrc
source ~/.zshrc
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