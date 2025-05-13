# Vim Motions & Commands Cheat Sheet

### command - count - motion

### **1. Text Objects and Motions**

- **Visual Select Inside**:

  - `vi(` / `vi)` / `vi{` / `vi}` / `vi"` / `vi'`: Select all text within `()`, `{}`, `""`, `''`, etc.
  - `vib`: Select all text within square brackets `[]`.
  - `viB`: Select all text within curly brackets `{}`.
  - `grn`: change word under cursor`{}`.
  - `norm`: `{}`.

- **Change Inside**:
  - `cib`: Delete everything inside `()` and enter insert mode.
  - `ciB`: Delete everything inside `{}` and enter insert mode.
  - `ciw`: Delete the current word and enter insert mode.
----

### **2. Visual Mode Commands**

- **Entering Visual Modes**:

  - `v`: Enter visual mode (character-wise).
  - `V`: Enter visual line mode.
  - `Ctrl + v`: Enter visual block mode.

- **Visual Block Mode**:
  - `I`: Insert text at the beginning of the block.
  - `A`: Append text to the end of the block.
  - Example:
    - `Ctrl + v` (visual block mode) → `I` → "enter some text" → `Esc`
    - Pair with: `gv` → `$` → `A` for appending text at the end.
----

### **3. Normal Mode Commands**

- **Text Manipulation**:

  - `~`: Toggle case for the selected character(s).
  - `df(`: Delete from the cursor to `(`, including `(`.
  - `dt(`: Delete from the cursor to `(`, excluding `(`.
  - `d$`: Delete from the cursor point to the end of the line.
  - `J`: Join two lines into one.

- **Movement**:

  - `%`: Jump to the matching parenthesis, bracket, or brace.
  - `{`: Move up by a paragraph.
  - `}`: Move down by a paragraph.
  - `w`: Move forward word by word.
  - `b`: Move backward word by word.
  - `e`: Jump to the end of the current word.
  - `_`: Jump to the start of the line.
  - `^`: Jump to the start of the line.
  - `$`: Jump to the end of the line.
  - `f<character>`: Jump to the next occurrence of the specified character on the current line.
  - `m+<any-alphabet>`: add a mark on the line ,represented by the alphabet provided.
  - `'` : list all the availables marks you can jump to.

- **Navigation**:
  - `gx`: Open the URL or link under the cursor.
  - `gf`: Open the file under the cursor.
  - `<line_number>G`: Jump to the specified line number.
  - `gg`: Move to the start of the file.
  - `G`: Move to the end of the file.
  - `Ctrl + d`: Move half a page down.
  - `Ctrl + u`: Move half a page up.
----

### **4. Visual Mode Tips**

- `gv`: Reselect the last visual selection.
- `I` (in visual block mode): Insert text before the block.
- `A` (in visual block mode): Append text after the block.
- **Quick Multi-Line Edits**:
  - Pair `gv` with `$` and `A` for efficient multi-line editing.

---
