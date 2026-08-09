# Lumide 0.19.0

- macOS only: Impeller is enabled since this version.

### Enhancements

#### Editor
- **Snippets support**: Create user or workspace TextMate snippets from the Command Palette, expand them alongside code completions, and move through placeholders with `Tab` or `Shift+Tab`. Plugins can also contribute snippets and file templates.
- Add support for Word Selection mode (double-click then drag) and Line Selection mode (triple-click then drag).
- Improve cursor movement, word selection/deletion, and extend selection actions to not be so greedy.
- Preserve completion popup upon typing.
- Highlight matches within completion popup.

#### New APIs support
- Upgrade to `lumide_api: 1.9.0`.
- Snippet contributions — Plugins can contribute TextMate-compatible JSON snippet files through `contributes.snippets`.

### Fixed
- Fix accepting code completions not applying required auto-imports.
- Fix macOS keyboard shortcut not working when combining with `Option` and/or `Shift` modifiers.
- Fix git repository and submodule label displaying absolute path on Windows.
- Fix cannot exit multi-cursor editing by pressing `Esc`.

---
Visit [lumide.dev](https://lumide.dev) for more.
