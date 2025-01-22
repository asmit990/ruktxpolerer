ruktxplorer

ruktxplorer is a terminal-based file explorer created with love by Asmit Pandey. Inspired by the NNN file manager, it uses Ratatui for the terminal UI and Crossterm for the terminal backend.

To traverse or not to traverse?

Features
Full CRUD operations on files and directories.
Move and copy files and directories.
Keyboard shortcuts for navigation and operations, ensuring a seamless experience without leaving the keyboard.
Traverse directly to a directory by typing its path.
Configurable options to tailor the experience to your needs.
Extract tar.gz or zip archives.
Bookmarks for your favorite directories.
Fuzzy finder for files in your current directory.
Preview files in the terminal.
Lightning-fast performance.
Installation
From Source

Install Rust.
Clone the repository:
git clone https://github.com/asmit990/ruktxplorer.git
Run cargo build --release.
The binary will be in target/release/ruktxplorer.
Add the binary to your system path.
From Cargo

Install Rust.
Run: cargo install ruktxplorer.
Ensure Cargo's bin directory is in your system path.
(Optional) Rename the binary to any name that suits you.
From Binary

Download the binary from the releases page.
Use chmod +x ruktxplorer (Linux/macOS only) to make the binary executable.
Move the resulting binary to your system path.
Usage
Run ruktxplorer in your terminal.

Keyboard Shortcuts
Navigation

ESC or q: Quit the application.
1: Select the Files pane.
2: Select the Directories pane.
j: Select the next item in the current pane.
k: Select the previous item in the current pane.
File and Directory Operations

n: Create a new file or directory, depending on the current pane.
CTRL + d: Delete the selected file or directory (to bin).
r: Rename the selected file or directory.
f: Navigate to a directory using a relative or absolute path.
x: Extract the selected archive to the current directory.
Move/Copy Operations

c: Append the selected file or directory to the move/copy buffer.
p: Open the move/copy buffer menu (Enter on any option is in relation to your current directory).
Fuzzy Finder Operations

w: Toggle FZF.
CTRL + n: 'Next' item in results.
CTRL + p: 'Previous' item in results.
Bookmark Operations

b: Show bookmarks menu.
z: Add the current directory to bookmarks.
CTRL + n: 'Next' bookmark in the menu.
CTRL + p: 'Previous' bookmark in the menu.
Help

?: Show help menu.
Configuration
The configuration file is located at /traverse/config.txt. Below is the default configuration for Asmit:

# Configuration for ruktxplorer by Asmit Pandey
show_hidden=true
excluded_directories=.git,.idea,.vscode,target,node_modules
The excluded directories are those that will not be searched when using the FZF. You can edit this list to add/remove directories as needed.

The bookmarks file is located at /traverse/bookmarks.txt. Here's an example for Asmit:

# Asmit's Favorite Directories
/home/asmit/projects
/home/asmit/music
/home/asmit/documents
Feel free to customize the configuration and bookmarks to suit your workflow!

This README format should now reflect the correct project name ruktxplorer and provide clear installation, usage, and configuration instructions. Let me know if you'd like any further edits!
