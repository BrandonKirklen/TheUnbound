# The Unbound

Campaign notes for **The Unbound**, an ongoing Dungeons & Dragons campaign set in the world of Exandria.

The party — Tomis (centaur cleric of the Matron of Ravens), Freya (half-orc zealot barbarian, the Cursed Zealot of the Black Crown), Grimbold (half-gnome / half-goblin spellcaster), Uriel (Scourge Aasimar horizon-walker ranger of the Earth Ashari), and Rowan Karst (steadfast son of Whitestone) — pursue the relics and threads of an age of warring gods across Whitestone, the Parchwood Timberlands, the Alabaster Sierras, and beyond.

## Layout

```
docs/
  Reference Notes/   - Character descriptions, world notes, set pieces, one-shot material
  Session Notes/     - One file per session (Session 0 through Session 118)
    TEMPLATE.md      - Copy this when starting a new session for consistent structure
mkdocs.yml           - MkDocs site configuration (Material theme)
.readthedocs.yaml    - Read the Docs build configuration
```

## Adding a new session

There are two paths:

- **From a transcript** — open this project in Claude Code and invoke the `dnd-unbound-session-notes` skill (lives at `.claude/skills/dnd-unbound-session-notes/SKILL.md`). It extracts a transcript into notes that match the established voice, structure, and proper-noun conventions.
- **By hand** — copy `docs/Session Notes/TEMPLATE.md` to `docs/Session Notes/Session N.md` and fill it in.

Either way, add a matching line to the `Sessions:` block in `mkdocs.yml`. The sidebar is ordered latest-first, so new entries go at the **top** of that block (immediately under `- Sessions:`).

## Browsing

- **GitHub** — read any file directly under [`docs/`](./docs/).
- **Hosted site** — published via [Read the Docs](https://readthedocs.org) using the configuration in `.readthedocs.yaml`.

## Building the site locally

```sh
python3 -m venv .venv
.venv/bin/pip install -r docs/requirements.txt
.venv/bin/mkdocs serve
```

Then open <http://127.0.0.1:8000>.

To produce a static build into `site/`:

```sh
.venv/bin/mkdocs build
```
