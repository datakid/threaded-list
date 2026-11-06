# Kashf

Arabic register of names in labelled groups. Each entry has a name, a class and a note.

## What it does

- Two views of the same data: a sheet, and a text view that uses `# Document title`, `== Group label` and `Name | Class | Note` lines.
- Imports CSV, JSON and TXT files. Modes are append after the current content, replace it, or merge by group label, with an optional source tag. A report lists the groups and names read and how many rows were skipped as blank, unparseable or under an unknown header.
- Flags duplicate names with a badge that jumps to them. The import report can remove duplicates.
- Exports JSON (recommended), CSV or TXT.
- Sixteen themes. Print options: freeze the header, pure black and white, and sources in print.
- Autosaves, keeps a history you can preview and restore, shows an undo toast for deletions, adds or removes several groups at once (`+3`, `-2`) and searches with `/`.

## What it does not do

- It has no accounts, sharing or sync. The register is kept in the browser's `localStorage`, and a warning appears if autosave fails because storage is full.
- It reads only `.csv`, `.json` and `.txt` files.
- It has no PDF export of its own. Printing uses the browser's print dialog.

## Network and install

Loads Google Fonts. It makes no other requests, and the register is not uploaded. Not installable; no service worker.

## Built with

One HTML file, with no build step and no framework. The interface is Arabic with an English switch.

## Run locally

Open `index.html` in a browser, or serve the folder with any static file server.
