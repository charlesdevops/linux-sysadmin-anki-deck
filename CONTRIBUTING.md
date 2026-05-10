# Contributing

Contributions are welcome. The goal of this deck is to be an accurate, focused resource for Linux system administrators and LFCS exam candidates. Quality matters more than quantity.

---

## How to Contribute

1. Fork the repository
2. Edit `LearningLinux/deck.json` directly (it is plain JSON — any text editor works)
3. Open a pull request with a clear description of what you changed and why

For larger changes, open an issue first to discuss the approach.

---

## What Is Welcome

- **Typo and grammar fixes** — spelling errors, awkward phrasing, broken HTML in any card
- **Technical corrections** — outdated flags, wrong syntax, commands that no longer work on modern distros
- **New cards on existing topics** — see the tag list in [README.md](README.md) for in-scope topics
- **English rewrites** — some cards may contain residual Italian-language content; English replacements are appreciated

## What Is Not Welcome

- Cards on non-Linux topics: Windows-only, macOS-only, or CMS/eCommerce platforms (WordPress, Magento, Drupal) without a clear Linux sysadmin angle
- Duplicate cards covering the same command or concept
- Stylistic rewrites without a technical reason

---

## Card JSON Format

New cards must follow one of the two existing note model formats.

**Code model** — for shell command knowledge:
```json
{
    "__type__": "Note",
    "fields": [
        "Your question here (HTML allowed)",
        "",
        "$ your-command here",
        "Optional notes, caveats, or references"
    ],
    "guid": "UniqueGuid10",
    "note_model_uuid": "55ed3f7c-4c87-11f1-853b-00090ffe0001",
    "tags": ["Linux", "YourTag"]
}
```

**Basic-Plus-Media model** — for cards with images or diagrams:
```json
{
    "__type__": "Note",
    "fields": [
        "Your question here",
        "",
        "Answer text here",
        "",
        "Optional notes",
        ""
    ],
    "guid": "UniqueGuid10",
    "note_model_uuid": "50780037-4c87-11f1-8d9c-00090ffe0001",
    "tags": ["Linux", "YourTag"]
}
```

Generate a unique `guid` using 10 random URL-safe characters (letters, digits, `!`, `#`, `$`, `%`, `&`). Use tags from the existing vocabulary in [README.md](README.md).

---

## Running the Cleanup Script

Before submitting a PR that modifies `deck.json`, you can run the cleanup script to verify your changes haven't introduced obvious issues:

```bash
python scripts/clean_deck.py
```

The script creates a backup (`deck.json.bak`) before making any changes.
