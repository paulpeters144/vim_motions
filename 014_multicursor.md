# Multicursor (multicursor.nvim)

Here are your configured shortcuts for `multicursor.nvim` based on your personal configuration:

## Your Shortcuts
- `<up>` / `<down>` : Add a cursor to the line above / below.
- `<leader>mn` : Match and add a cursor to the **next** occurrence of the word/selection.
- `<leader>ms` : **Skip** the next occurrence (moves to the next match without adding a cursor).
- `<leader>ma` : Match **all** occurrences of the word in the buffer.
- `<leader>ml` : **Align** all active cursors.
- `<leader>mx` : Delete the current main cursor (only when multiple cursors are active).
- `<left>` / `<right>` : Cycle your main cursor between the active cursors.
- `<Esc>` : Enable/Clear cursors.

## Exercise: Match, Skip, Rename, and Align

**Goal:** Change the `var` keywords to `const` (skipping the one for `age`), and then align the `=` signs for cleaner formatting.

**Steps:**
1. Place your cursor on the very first `var` keyword.
2. Press `<leader>mn` twice to select the first and second `var`.
3. Press `<leader>ms` to **skip** the third `var` (we want `age` to stay mutable!).
4. Press `<leader>mn` to select the fourth `var`.
5. Press `cw` (change word), type `const`, and press `<Esc>` to return to Normal mode.
6. Press `<Esc>` again to clear all your cursors.
7. Move your cursor to the first `=` sign.
8. Press `<down>` three times to add a cursor to each `=` sign on the lines below.
9. Press `<leader>ml` to align all the `=` signs perfectly.
10. Press `<Esc>` to clear your cursors.

```javascript
var firstName = "Alice";
var lastName = "Smith";
var age = 30;
var occupation = "Engineer";
```
