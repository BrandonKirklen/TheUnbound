# The Unbound

Campaign notes for **The Unbound**, an ongoing Dungeons & Dragons campaign set in the world of Exandria.

The party — Tomis (centaur cleric of the Matron of Ravens), Freya (half-orc zealot barbarian, the Cursed Zealot of the Black Crown), Grimbold (half-gnome / half-goblin spellcaster), and Uriel (Scourge Aasimar horizon-walker ranger of the Earth Ashari) — pursue the relics and threads of an age of warring gods across Whitestone, the Parchwood Timberlands, the Alabaster Sierras, and beyond.

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

Copy `docs/Session Notes/TEMPLATE.md` to `docs/Session Notes/Session N.md`, fill it in, then add a matching line to the `Sessions:` block in `mkdocs.yml`.

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
