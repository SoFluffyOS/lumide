# Lumide 0.9.0

### Enhancements

#### C.O.R.G.I (Git)
- Add responsive center-pane detail tabs for compact Git (C.O.R.G.I.) and Plugins panes.
- Improve C.O.R.G.I. commit inspector with a more compact layout and clearer modified-file summary.
- Group nested folders in C.O.R.G.I. tree file views for shorter, easier-to-scan file lists.

#### Files
- Make File Tree toolbar always visible (no longer requires hover).
- Add workspace name display to File Tree toolbar.
- Add list/tree view toggles, status badges, filtering, and keyboard navigation to C.O.R.G.I. changed-file lists.

#### Editor
- Highlight selected text occurrences in the editor.
- Improve search match highlighting in the editor.

#### Flexible Pane System
- Support customizing tab bar placement.
- Improve Runtime Control popup:
  - Reorder Plugins tab to show "Available" before "Waiting for Activation".
  - Add sticky "Manage Plugins" at the footer.

### Fixed
- Fix git indicator overlapping with tree content.
- Keep File Tree item icon and text colors unchanged when selected.
- Improve editor Back/Forward navigation history to preserve forward entries and avoid duplicate stops.
- Increase bracket matching limits for larger files and long logical lines.
- Prefer the outermost fold region when multiple Flutter-style widget constructors start on the same line.
- Place Git blame ghost text after folded line placeholders instead of inside the folded region.

---
Visit [lumide.dev](https://lumide.dev) for more.
