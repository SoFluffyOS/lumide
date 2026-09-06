# Lumide 0.21.0

### Enhancements

I've replaced all `figma_squircle` usages with Flutter's built-in `RoundedSuperellipseBorder`. You'll see slightly performance improvement across the editor. Thanks to [@rydmike](https://github.com/rydmike) for his [squircle_study](https://github.com/rydmike/squircle_study).

#### SDK Manager
- Introducing SDK Manager with built-in Dart SDK management.
- Plugins can leverage the new APIs to use the same SDK management UI. (E.g: `lumide_flutter` uses this to manage Flutter versions).

#### Editor
- Allow to switch between Subtle or Eager modes for AI Completion. Subtle mode default to use Alt/Option key to show the AI suggestion.

#### Terminal
- Add Terminal Profiles configurations (Settings > Terminal).
- Allow to quickly open any Terminal profile within Add Pane > Terminal expanded menu.

#### Settings
- Add Theme/Color Scheme Preview.
- Enable soft wrap by default for Markdown files (`.md`, `.mdx`, `.markdown`).
- Support per-language settings overrides for 35 additional languages in Editor and Vim settings scopes: Batch, CMake, CSS, Dockerfile, Dotenv, Elixir, Erlang, Groovy, Haskell, HTML, INI, JavaScript React (JSX), JSON, Kotlin, Lua, Makefile, Markdown, Nix, Objective-C, Objective-C++, PowerShell, Protocol Buffers, R, Ruby, Scala, SCSS, Shell Script, SQL, Svelte, TOML, TypeScript React (TSX), Vue, XML, YAML, and Zig.

#### New APIs support
- Upgrade to `lumide_api: 1.10.0`.
- Add `workingDirectory` param for shell spawn API.
- Allow plugins to be started manually from Plugin Manager.

### Fixed
- Fix environment variables not detected in some cases.
- Fix context menu description overflow.
- Fix YAML syntax highlighter mistakenly treating asterisks in file globs and paths (e.g. `**/*.dart`) as anchor/alias tokens.
- Fix C.O.R.G.I commit message & Agent Chat input content getting lost upon tab switching.

---
Visit [lumide.dev](https://lumide.dev) for more.
