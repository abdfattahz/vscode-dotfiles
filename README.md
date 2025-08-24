# 📖 VS CodeVim Custom Keybindings Cheatsheet

This repo contains my personal VS Code + Vim keybindings configuration.  
The tables below show all custom mappings grouped by category, with plain-English descriptions.

---

## 🟦 Basic Indenting / Tab Fixes

| Keys        | Action     | When                                            |
| ----------- | ---------- | ----------------------------------------------- |
| `Tab`       | Insert tab | While editing text, when Tab doesn’t move focus |
| `Shift+Tab` | Outdent    | While editing text, when Tab doesn’t move focus |

---

## 🧭 Navigation (Vim-aware)

| Keys        | Action                                  | When                                                           |
| ----------- | --------------------------------------- | -------------------------------------------------------------- |
| `Ctrl+H`    | Focus **left** editor group             | In Normal mode, multiple editor groups open                    |
| `Ctrl+H`    | Previous editor                         | In Normal mode, only one editor group open                     |
| `Ctrl+L`    | Focus **right** editor group            | In Normal mode, multiple editor groups open                    |
| `Ctrl+L`    | Next editor                             | In Normal mode, only one editor group open                     |
| `Ctrl+K`    | Navigate **up** among UI panes          | Always                                                         |
| `Ctrl+J`    | Navigate **down** among UI panes        | Always                                                         |
| `Space ,`   | Show all open editors (buffers list)    | In Normal mode, editor focused or no input box focused         |
| `Space e`   | Toggle sidebar + focus Explorer         | In Normal mode, editor focused and sidebar not already focused |
| `Space e`   | Toggle sidebar + return focus to editor | When sidebar is focused                                        |
| `Space e`   | Hide sidebar if Explorer visible        | In Normal mode, editor focused and Explorer visible            |
| `Space s h` | Split editor vertically (to right)      | In Normal mode, editor focused                                 |
| `Space s v` | Split editor horizontally (down)        | In Normal mode, editor focused                                 |

---

## ✍️ Coding Helpers

| Keys           | Action                             | When                                                            |
| -------------- | ---------------------------------- | --------------------------------------------------------------- |
| `Space c a`    | Code Actions / Quick Fix           | In Normal mode, editor focused                                  |
| `Shift+K`      | Move selected line(s) up           | In Visual Line mode                                             |
| `Shift+J`      | Move selected line(s) down         | In Visual Line mode                                             |
| `Ctrl+Shift+K` | Show Hover (docs/types)            | In Normal mode, editor focused                                  |
| `Space c r`    | Rename symbol                      | In Normal mode, editor focused                                  |
| `Space c s`    | Go to symbol in file               | In Normal mode, editor focused                                  |
| `Space b d`    | Close current editor               | In Normal mode (editor focused) or no input box active          |
| `Space b o`    | Close other editors                | In Normal mode (editor focused) or no input box active          |
| `Space Space`  | Quick Open (file search)           | In Normal mode, editor focused or no input box active           |
| `Space g d`    | Go to Definition                   | In Normal mode, editor focused                                  |
| `Space g r`    | Find References                    | In Normal mode, editor focused                                  |
| `Space g i`    | Go to Implementation               | In Normal mode, editor focused                                  |
| `Space s g`    | Global Search (Find in Files)      | In Normal mode, editor focused or no input box active           |
| `Space g g`    | Open Git Source Control view       | In Normal mode, editor focused or no input box active           |
| `Ctrl+N`       | Add next occurrence (multi-cursor) | In Normal or Visual mode, editor focused or no input box active |

---

## 📁 File Explorer

| Keys         | Action                                    | When                                           |
| ------------ | ----------------------------------------- | ---------------------------------------------- |
| `Ctrl+Alt+O` | Open folder dialog                        | Always                                         |
| `R`          | Rename item                               | In Explorer, item selected (not root/readonly) |
| `C`          | Copy item                                 | In Explorer, item selected (not root/readonly) |
| `P`          | Paste item                                | In Explorer, focus inside Explorer             |
| `X`          | Cut item                                  | In Explorer, item selected (not root/readonly) |
| `D`          | Delete item                               | In Explorer, item selected (not root/readonly) |
| `A`          | New file                                  | In Explorer, folder selected                   |
| `Shift+A`    | New folder                                | In Explorer, folder selected                   |
| `S`          | Open file to the side                     | In Explorer, file selected                     |
| `Shift+S`    | Split below → open → focus → close others | In Explorer, file selected                     |
| `Enter`      | Open file and focus editor                | In Explorer, file selected (not folder)        |
| `Enter`      | Expand/collapse folder                    | In Explorer, folder selected                   |

---

## 🐞 Debugging

| Keys        | Action                 | When                                                               |
| ----------- | ---------------------- | ------------------------------------------------------------------ |
| `Space d a` | Select and start debug | In Normal mode, editor focused or no input box, debugger available |
| `Space d t` | Stop debugging         | In Normal mode, editor focused, debugging active                   |
| `Space d o` | Step Over              | In Normal mode, editor focused, debugger stopped                   |
| `Space d b` | Toggle breakpoint      | In Normal mode, editor focused                                     |
| `Space d e` | Show debug hover       | In Normal mode, editor focused, debugging stopped                  |
| `Space d c` | Continue               | In Normal mode, editor focused, debugging stopped                  |

---

## ℹ️ Notes

- Many bindings are **Vim-aware**, meaning they only work in `Normal` or `VisualLine` mode.
- Some Explorer bindings are single letters (`R`, `C`, `D`, etc.) but only apply **inside the File Explorer**, so they won’t interfere with normal editing.
- `Ctrl+K` has been repurposed for pane navigation (this disables VS Code’s default `Ctrl+K ...` chord system).

---
