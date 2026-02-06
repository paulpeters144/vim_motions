# Getting Started with Neogit & Git Integration

This guide will help you get up to speed with the Git tools now configured in your Neovim setup.

## 1. The Powerhouse: Neogit (`<leader>gg`)
Neogit is an interactive Git interface inspired by Magit. It allows you to perform almost all Git operations without leaving Neovim.

### Basic Workflow
1.  **Open Neogit**: Press `<leader>gg`.
2.  **Staging**: Move your cursor over a "Unstaged" file or hunk and press `s` to stage it. Press `u` to unstage.
3.  **Committing**: Press `c` to open the commit menu, then `c` again to create a commit. Write your message and use `:wq` to finish.
4.  **Pushing/Pulling**: Press `p` for the push menu or `f` for the fetch/pull menu.
5.  **Closing**: Press `q` to exit the Neogit buffer.

---

## 2. Advanced Diffing: Diffview (`<leader>gd`)
When you need to review a large set of changes across the whole project.

*   **`<leader>gd`**: Opens a dedicated tab with a file tree on the left and a side-by-side diff on the right.
*   **`<leader>gh`**: Opens the history of the **current file**. You can scroll through previous versions and see exactly what changed in each commit.
*   **Close**: Type `:DiffviewClose` or close the tab.

---

## 3. Inline Magic: Gitsigns (`<leader>h`)
Gitsigns works while you are coding in any file. Look for the `+`, `~`, or `_` in the gutter.

### Quick Navigation
*   **`]h`**: Jump to the next change.
*   **`[h`**: Jump to the previous change.

### Hunk Actions
*   **`<leader>hp`**: **Preview** the change in a floating window. This is the fastest way to see what you just deleted or changed.
*   **`<leader>hs`**: **Stage** just the hunk under your cursor.
*   **`<leader>hr`**: **Reset** (undo) the hunk under your cursor.
*   **`<leader>hb`**: **Blame** line. See who changed this line and why in a detailed popup.

---

## 4. Quick Search: Telescope (`<leader>gs`)
If you just want to find which files you've touched:
*   **`<leader>gs`**: Opens a searchable list of changed files with a live preview of the diff.

## Summary Cheat Sheet
| Keybind | Action | Tool |
| :--- | :--- | :--- |
| `<leader>gg` | Open Git Status UI | Neogit |
| `<leader>gd` | Open Project Diff | Diffview |
| `<leader>gh` | File History | Diffview |
| `<leader>gs` | Search Changed Files | Telescope |
| `]h` / `[h` | Next/Prev Change | Gitsigns |
| `<leader>hp` | Preview Change | Gitsigns |
| `<leader>hb` | Blame Line | Gitsigns |
| `<leader>tb` | Toggle Inline Blame | Gitsigns |
