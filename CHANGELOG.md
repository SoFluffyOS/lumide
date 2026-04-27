# Lumide v0.3.0

### Enhancements
- **Linux Auto-Update**: Full support for in-app automatic updates on Linux. *Note: If you are upgrading from version `0.2.0`, please re-run the `curl -f https://lumide.dev/install.sh | sh` installation script once to receive the new auto-updater. Future updates will be applied automatically from within the IDE.*
- **Enhanced Dart SDK Support**: Native support for FVM, Puro, and custom paths. The IDE now automatically detects project-specific environments (like `.fvmrc`) and offers simplified configuration during initial setup.
- **Improved Markdown Preview**: Significantly better rendering for SVG badges and diagrams. Added support for inline SVGs, relative image paths, and working local file links.
- **New Help Menu**: Added quick access to documentation, keyboard shortcuts, and issue reporting directly from the platform menu bar.
- **Enhanced Release Notes**: Better visibility for version history and update information within the IDE.
- **Install Lumide CLI**: Easily install the Lumide command-line interface to your system PATH via the Lumide menu.
- **Command Line Support**: You can now launch Lumide with a specific folder path as an argument.

### Fixed
- **Windows Reliability**: Fixed critical issues with file path resolution on non-system drives and improved detection of system environment variables.

---
Visit [lumide.dev](https://lumide.dev) for more.
