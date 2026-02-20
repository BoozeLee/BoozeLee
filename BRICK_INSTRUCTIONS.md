# BRICK INSTRUCTIONS
*Marco-o1 - 2026-02-20*

## What This Repo Does
View the profile for project updates and contributions.

## Price
$0

## Brick Type
Developer Profile

## Gumroad Copy
Explore the projects of developer Kiliaan Van Voorden.

## Build
```bash
source ~/Energetic_Lexicon/.venv/bin/activate
pyinstaller --onefile --name BoozeLeeBrick --collect-all rich --copy-metadata rich codex_brick.py
```