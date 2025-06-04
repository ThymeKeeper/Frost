# ❄️ Frost

A blazingly fast, lightweight, Terminal User Interface (TUI) IDE for Snowflake, built with Rust. Navigate your data warehouse, execute queries, and analyze results - all from the comfort of your terminal.

### Core Functionality
- **Full SQL Editor** with syntax highlighting, find/replace, and bracket matching
- **Multi-tab Results** - Run a series of queries and switch between all returned result sets
- **Schema Navigator** - Browse databases, schemas, tables, and columns
- **Role-based Access** - Switch between Snowflake roles without leaving the IDE
- **Smart Query Execution** - Run selected text or query at cursor with `Ctrl+Enter`
- **Large Result Handling** - Smoothly handles tens of millions of returned rows using tile-based storage

### Editor Features
- Syntax highlighting for SQL keywords, strings, numbers, comments
- Bracket matching and auto-indentation
- Find and replace strings within the buffer
- Selection modes (rectangular, line, column)
- Undo/redo
- Session recovery and autosave

### Results Viewer
- Column, row, and rectangular selection modes
- Export to CSV
- Copy selections to clipboard
- Find strings within result sets
- Quck Statistical summaries of selected data
- Null value detection and handling

### DB Navigator
- Full file tree exploerer for all available databases
- Toggle secondary role access
- View database tree by role
- Insert table and columns into the editor
- Find matching strings within the navigator

### Other Features
- **Batch Mode** - output a batch file to automate running sql files
- **Background Schema Crawler** - Keeps schema information up-to-date
- **Configurable Themes** - Customize colors via TOML configuration

## Screenshots

![screenshot1](https://github.com/user-attachments/assets/396baa71-a344-4374-812d-7de61fdb6b49)

![screenshot2](https://github.com/user-attachments/assets/3088c40d-a3e6-4d85-8c51-4c1a27c7fa3a)

### Notes
- Build with "cargo build --release --bins ; if ($?) { cargo run --release }"
- Best viewed with a nerd font such as FiraMono.
- If you come across any rendering glitches, double tap F1 to re-draw the screen.
- This has only been tested in Windows Terminal, though there is some untested Ubuntu support built in.
