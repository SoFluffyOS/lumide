# Lumide 0.25.0

Your code lives on a board now, your agents work together, and you can try Lumide with Dart and Flutter in your browser at [dartpad.lumide.dev](https://dartpad.lumide.dev).

Lumide needs macOS 12 Monterey or later. On macOS 10.15 or 11, keep 0.21.0.

### Enhancements

#### 🌐 DartPad
- **[DartPad](https://docs.lumide.dev/workspace/dartpad)**: Lumide in your browser, no install, no server. Dart and Flutter with pub.dev packages, real analysis, Run, hot reload and DevTools. Open any GitHub repo, package or Gist, and take it home as a zip.

#### 🦉 Layout
- **[O.W.L.](https://docs.lumide.dev/workspace/split-panes)** (Overview With Links): Lay your code out on a board. A pane opened from another lands beside it, linked, so the path you took stays in view.
- **[Focus Mode everywhere](https://docs.lumide.dev/workspace/split-panes)**: `Shift + Esc` fills the window with the focused pane, in any layout. Hold it to peek.
- **[Switch frames](https://docs.lumide.dev/workspace/split-panes)** with `Ctrl + Tab`, the most recent first.
- **[Where Panes Open](https://docs.lumide.dev/getting-started/interface)**: Code-first or Agent-first.
- **Editor header**: Every editor names its file's path. Click a folder in it to browse.
- Narrow windows keep the title bar tidy, with a `⋯` for what doesn't fit.

#### 🤖 Agents
- **[Chats in a worktree](https://docs.lumide.dev/ai#chats-in-a-worktree)**: Each chat gets its own Git worktree and branch, so agents never touch your checkout. Apply, merge or open a pull request when it's done.
- **[Chats agents start](https://docs.lumide.dev/ai#chats-agents-start)**: An agent starts other chats, with any agent, and hears back when they finish. Claude Code asking Codex to review its diff, say.
- **[Lumide's tools for agents](https://docs.lumide.dev/ai)**: Rename, format, fix problems, find references, run tests, debug, read your terminals and drive an iOS Simulator, through Lumide instead of `sed`.
- **Agents sidebar**: Every chat in one place, with what each is doing, plus the coding agents running in your terminals. **[Usage](https://docs.lumide.dev/ai)** shows today's spend and how close you are to a rate limit.
- **[Plan review](https://docs.lumide.dev/ai)**: Read an agent's plan as a document before any code is written, and comment on it.
- **Review what agents change**, even files a command like `sed` changed, in one editable scroll, with Accept and Reject per file or hunk.
- **[Files kept from AI](https://docs.lumide.dev/ai)**: `.env` files and private keys never reach completions, commit messages or Agent Chat. Add your own in a `.aiignore`.
- **MCP Servers**: See every server your agents get, from every workspace folder, each checked for its tools.
- **[Environment variables](https://docs.lumide.dev/ai)** for agents: a value from the keychain, or a command such as `gh auth token`.
- Allow a command by its leading words, such as `flutter test`, for this workspace or everywhere.
- Send the problems a turn left behind back to the agent in one click, or automatically.
- A notification when a chat needs you, finishes or fails.

#### 💬 Agent Chat
- **Reads like a document**: Replies without bubbles, one message box, cards that ask and then fold away, and a turn that folds into "Worked for 2m · Changed 4 files".
- **Smarter `@` mentions**: Open files, problems, uncommitted changes, terminals and web pages, as chips. Paste a screenshot as a picture, or code as a snippet.
- **A new chat knows where it is**: Fix N problems, Review N changed files, or Explain the open file, in one click.
- **Follow the agent** as it reads and edits, right at the line.
- Commands run live in terminal cards, and subagents show as cards with Stop and their whole transcript.
- Ghost-text completions, Up for your last messages, a chat remembers its mode and model, and closing a busy chat asks first.
- Chats you started with `claude` or `codex` in a terminal show up too. Continue them in either place.

#### 🦝 Raccoon & Flutter
- **More sizes, one run**: Add View At shows your app at another size on the board, all reloaded together. Instant on macOS and Linux.
- **A phone, not a desktop**: Appearance, text size, language, rotation, touch, an on-screen keyboard, deep links and push notifications. Plugins with no desktop version answer as a phone would.
- **[Design Mode](https://docs.lumide.dev/ai#design-mode-for-flutter-apps)**: Click a widget and it lands in Agent Chat, with its picture and code.
- **Agents use your app**: `raccoon_find` and `raccoon_input` tap, type and scroll by widget, and `flutter_reload` hot reloads after an agent's edit.
- **[iOS Simulator in a frame](https://docs.lumide.dev/languages/flutter-and-dart)** (macOS): Boot a simulator right beside your code, no Simulator app. Slim This Sim cuts its memory to a quarter.
- One-click Raccoon setup from Runtime Control, and fast runs that compile nothing by default.
- **[Color and icon previews](https://docs.lumide.dev/editor)**: A swatch with a color picker before each color, and Flutter's icons right in the code.

#### 📝 Markdown & HTML
- **Lumide's own Markdown engine**: Renders like GitHub, alerts included, and long files scroll smoothly. Agent Chat messages take about half the memory.
- **Edit in the preview**, with a formatting toolbar and the shortcuts you know. Off by default.
- Copy tables into Docs, Notion or Sheets the right way, and zoom into big Mermaid diagrams.
- **[HTML Preview](https://docs.lumide.dev/editor/html-preview)**: Preview HTML beside the editor, drawn without a WebView, with an inspector that jumps to the source.

#### ✏️ Editor & Workspace
- **[New Project](https://docs.lumide.dev/workspace/workspaces#creating-a-project)**: Templates for Dart, a static site or a Lumide plugin, plus the ones your plugins add.
- **[Next edits](https://docs.lumide.dev/ai)** with GitHub Copilot: Predictions that change and remove code, shown beside it.
- **[Bookmarks](https://docs.lumide.dev/navigation)**, a **[TODOs](https://docs.lumide.dev/navigation/project-search)** pane, **[filtered Problems](https://docs.lumide.dev/languages/diagnostics-and-problems)** and a sharper **[Diff pane](https://docs.lumide.dev/git/diff-viewer#the-diff-pane)**.
- **[Rename in the Files pane](https://docs.lumide.dev/getting-started/interface)**, with the imports that name the file updated.
- **[Local History](https://docs.lumide.dev/workspace/local-history)**: Every change and who made it, you or an agent. Restore in one step.
- **[Settings](https://docs.lumide.dev/customization/settings)**: Reorganized, with a search that narrows the sidebar.
- **[Python versions](https://docs.lumide.dev/customization/sdk-manager)** per folder with the Python plugin, and Gauge specs highlighted.
- **[Plugin updates](https://docs.lumide.dev/plugins)** checked on startup, with Update All.
- **[Reduce Motion](https://docs.lumide.dev/customization/themes)**, and spinners that use far less CPU.
- C.O.R.G.I.: Up brings back recent commit messages, and Review Changes reads any commit in one scroll.
- **[Smaller macOS download](https://docs.lumide.dev/getting-started/installation)**: 22 MB for your Mac instead of 63 MB.

#### 🧪 Experimental
- **[Built-in Browser](https://docs.lumide.dev/editor/html-preview#browser-panes)**: Browse your dev server right in Lumide, and let agents click through it. Off by default for now, as a heavy page can freeze Lumide. Turn it on in **Settings → Editor → HTML Preview**.

#### 🔌 New APIs support
- `lumide_api: 1.14.0`: Plugins follow your agents (`context.agents`), test runs (`tests.onDidEndRun`) and window focus (`window.onDidChangeFocus`).

### Fixed
- Renaming `readme.md` to `README.md` works on macOS and Windows.
- **VS Code keymap**: Go Back and Go Forward use VS Code's keys on every platform.
- **Copy as HTML** pastes as formatted content into Docs, Notion or Mail.
- Typing `I'm` no longer adds a closing quote.
- `Ctrl + backtick` brings up the terminal wherever it lives, and hides it again.
- Commands an agent runs report their real output and exit code, with pagers off.
- Rejecting an agent's changes keeps your own edits made since.
- **Revert Here** asks first, can be undone for 10 seconds, and tells the agent what was undone.
- Copying a long terminal command copies all of it.
- Mouse drags reach terminal apps that use the mouse.
- Idle background terminal tabs no longer spin.
- Quitting gives plugins time to stop their servers and apps.
- Agent Chat's Session Config bar is back for Claude.
- Agent comments leave the pending list once sent.
- Old changes no longer show as pending when you reopen a chat, and Reject All fully restores a file changed several times.
- Status bar rings match the text beside them.

---
Visit [lumide.dev](https://lumide.dev) for more.
