# Oshorial Lore Wiki

This repository contains the source for the Oshorial campaign wiki, built with MkDocs and the Material theme.

## What You Need

- Python 3.10 or newer
- `pip`
- A terminal on macOS or Windows

## Run Locally on macOS

1. Open Terminal and change into the repository:

```bash
cd /Users/patrickfaulkner/Documents/repos/oshorial-lore-wiki
```

2. Create and activate a virtual environment:

```bash
python3 -m venv .venv
source .venv/bin/activate
```

3. Install the dependencies:

```bash
pip install -r requirements.txt
```

4. Start the local documentation server:

```bash
mkdocs serve
```

5. Open the site in your browser at:

```text
http://127.0.0.1:8000
```

## Run Locally on Windows

1. Open PowerShell or Windows Terminal and change into the repository:

```powershell
cd C:\Users\<your-username>\Documents\repos\oshorial-lore-wiki
```

2. Create and activate a virtual environment:

```powershell
py -3 -m venv .venv
.\.venv\Scripts\Activate.ps1
```

If PowerShell blocks activation scripts, run this once in the same terminal first:

```powershell
Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass
```

3. Install the dependencies:

```powershell
pip install -r requirements.txt
```

4. Start the local documentation server:

```powershell
mkdocs serve
```

5. Open the site in your browser at:

```text
http://127.0.0.1:8000
```

## Useful Commands

Build the static site without serving it locally:

```bash
mkdocs build
```

## Content Layout

- `docs/index.md` - Home page
- `docs/locations/` - Location pages
- `docs/npcs/` - NPC pages
- `docs/players/` - Player character pages

## Notes

- If you add new pages, update `mkdocs.yml` so they appear in the navigation.
- Keep the virtual environment out of version control; `.venv/` is already a local-only setup step.