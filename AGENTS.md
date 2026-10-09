# books

Bedrock add-on (BP-only, **no `RP/`**) with Catholic prayer and catechism books
in Polish. min_engine 1.20.0, version 1.0.3.

## No namespace

This project has **no custom namespace and no `config.json`.** Every identifier
is `minecraft:written_book`; the books are distinguished by loot table, not by
identifier. Don't look for `bridge:` here — it does not appear anywhere.

## Content

`BP/loot_tables/katechizm.json` — 9 separate pools:
Evangelical blessings, virtues, sins against the Holy Spirit, five conditions of
good confession, the commandments (god's / church / love), seven deadly sins,
six truths of faith.

`BP/loot_tables/modlitwy.json` — 6 pools:
Act of faith, Guardian Angels, Angelus, Our Father, Hail Mary, Creed.

## Distribution

```
/loot give @s loot katechizm
/loot give @s loot modlitwy
```
Each book is its **own pool** with `"rolls": 1`, so one `/loot give` returns all
books in the group — 9 or 6 respectively. That is a consequence of the table
structure, not of any explicit "give everything" setting.

There is **no `BP/functions/` and no `.mcfunction` files** — players or
command blocks type the `/loot give` command themselves.

## Conventions

- Loot table filenames are lowercase ASCII without Polish diacritics
  (`katechizm.json`, `modlitwy.json`).
- `BP/manifest.json` has `"dependencies": []` — the absent RP is intentional.
- Translations `["en_US", "pl_PL"]`.

## Known issues

- **The UUIDs are hand-written placeholders**
  (`a1b2c3d4-e5f6-4a5b-8c9d-…` for the pack, `b2c3d4e5-f6a7-…` for the module),
  not generated. Changing them invalidates existing installs.
- `LICENSE` is plain MIT for the whole project. Any claim that code and prayer
  text are licensed separately is **an interpretation, not written down**.
- `verify_project_structure` treats `RP/` as required, so this project always
  reports a missing RP. Expected — don't add an RP just to silence it.
- `verify_all.py` is byte-identical to the one in `just-clock`.