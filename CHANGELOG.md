# Lumide 0.20.0

I have explicitly disabled Impeller on all supported platforms due to rendering issues.

### Enhancements

#### Editor
- **Vim Mode support**: Enable in Settings > Vim > Vim Mode. If you don't want Vim Mode at all, can disable it within Plugin Manager.

#### Plugin Marketplace
- Add new categories: Snippets, Utilities.

#### New APIs support
- Upgrade to `lumide_api: 1.9.0`.
- Snippet contributions — Plugins can contribute TextMate-compatible JSON snippet files through `contributes.snippets`.

### Fixed
- Fix blank screen upon open on Linux.
- Preserve the cursor's Y position when moving Up/Down across empty lines.
- Fix Project Search sometimes not scroll to search match within Preview panel.

---
Visit [lumide.dev](https://lumide.dev) for more.
