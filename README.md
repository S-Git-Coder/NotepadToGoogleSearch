
# NotepadToGoogleSearch

A Node.js utility that monitors a local notepad.txt file and automatically performs a Google search in Chrome whenever the file content changes. Useful for quickly searching text written in Notepad or any text editor.

## Features

- Monitors notepad.txt for changes.
- Debounces rapid changes (waits 5 seconds after last edit).
- Validates input (ignores empty, too short, too long, or duplicate queries).
- Automatically opens Google search in Chrome for new queries.
- Simple web interface (index.html) to show monitoring status.

## How It Works

1. Edit and save text in notepad.txt.
2. The server detects changes and, after a short delay, opens a Google search for the new content in Chrome.
3. The web interface polls the server for updates and can open the search in a new tab.

## Installation

1. Clone this repository.
2. Install dependencies:
   ```sh
   npm install
   ```
3. Start the server:
   ```sh
   npm start
   ```
4. Edit notepad.txt and watch your browser open Google searches automatically.

## Requirements

- Node.js
- Google Chrome installed and available in your system PATH (for `start chrome` command on Windows).

## File Structure

- server.js - Main Node.js script for file monitoring and search logic.
- notepad.txt - The file you edit to trigger searches.
- index.html - Simple web page for status display.
- package.json - Project metadata and dependencies.

## License

ISC

---

You can copy and upload this as your `README.md` on GitHub. Let me know if you want to customize or add more details!
