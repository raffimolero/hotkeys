# VSCode cheat sheet

# Hand Positions

Movement position:
- Left pinky on Ctrl and ready index/middle for Ctrl+W/E/A/S/D/Z/X/C/V/U/1/2
- Left Ring on Shift and ready for Ctrl+Shift
- Left thumb on Space for comfort, but ready for **Alt**+Tab/1/2/3/...
- Place Right hand on Up/Down/Left/Right (I personally use Right thumb for Down) and ready for Backspace/Ins/Del/Home/End/PgUp/PgDn

Selecting by line:
- first press Home or End
- now only press Shift+Up/Down
  - press Home or End again before doing anything

# Opening a file/folder/project:
- Ctrl+R => search and open from recent projects
- Ctrl+O => open file from file explorer
- (in terminal) `code <path>` => opens <path> in VSCode
  - `code` must be in your system PATH
  - may open in current window or new window depending on configuration

# Show Keybinds:

- Ctrl+K+S and it will show you every keybind that exists and can exist

# Motions:

- Ctrl+U => cursor undo
- Ctrl+Alt+U => cursor redo
- Ctrl+Left/Right => move cursor left/right by word
- Ctrl+Up/Down => scroll up/down
- PgUp/PgDn => page up/down
- Home/End => goto start/end of indented line (Press Home twice to ignore indent)
- Ctrl+Home/End => goto start/end of file
- Shift+<motion> => extend selection
- Alt+Shift+Left/Right => move up/down syntax tree
  - e.g. Alt+Shift+Right will progressively select: word -> line -> if block -> if/else block -> function body -> whole function -> etc
- Ctrl+F then Alt+L then type => search for text (press Alt+L BEFORE typing the search string. this restricts search within selection. they should just make that the default...)
  - Alt+R => toggle regex
  - Enter => next occurrence
  - Shift+Enter => previous occurrence
  - Alt+Enter => Create a new multicursor selection on every occurrence

# Text and Code editing:

- Ctrl+X/C/V => cut/copy/paste
  - operates on whole line if there is no selection.
- Backspace goes left, Del goes right, Ctrl+ also works to delete by word
- if you're on mac, use alt (aka option) instead of Ctrl and fn+Delete for Del
- Ctrl+. => "quick fix" (language server)
  - can autocomplete your code or refactor or whatever to help you
- Ctrl+<space> => show code suggestions/autocomplete pane
- F2 => rename symbol
- F12 => goto definition
- Shift+F12 => goto references
- Ctrl+/ => comment/uncomment
- Shift+Alt+A => block comment for those who really need it

# Tab/Panel Navigation

  - Ctrl+` => open/close terminal
  - Ctrl+W => close current tab (closes panel if no tabs remain)
  - Ctrl+Tab => or Ctrl+PgDn switch to next tab in the current panel
  - Ctrl+Shift+Tab or Ctrl+PgUp => switch to previous tab in the current panel
  - Alt+1/2/3/... => switch to a specific tab
  - Ctrl+\ => open a new panel pointing to the current file
  - Ctrl+Alt+Left/Right => Move current tab to the next panel left/right
  - Ctrl+1/2/3/... => switch to a specific panel
  - Ctrl+E/P => search and open file by name
  - Ctrl+Shift+E => select File Explorer
    - Up/Down => navigate between files
    - Left/Right => collapse/expand folder
    - Enter => open file (possibly in new tab) in current panel
    
# Multiple Cursors

Reminder:
- Ctrl+U => cursor undo
- Ctrl+Alt+U => cursor redo

- Ctrl+D => create new multicursor on next occurrence
- Ctrl+K then Ctrl+D => skip the CURRENT occurrence, instead select next one
- Ctrl+Alt+Up/Down => new cursor on the line above/below
  - you can rebind this if it does something else for you (mac uses option+cmd instead of Ctrl+Alt, my linux also used to flip to a different desktop)
  - the new cursor will select the same span of text if possible
- Esc => one of the following:
  - if multicursor, delete all selections except primary
  - else if there is a selection, clear selection
  - else if searching, cancels Ctrl+F search
  - else idk

# Code Folding (Expand/Show or Collapse/Hide block)

- Ctrl+K+0 will fold all your code recursively, so you can see the structure
- Ctrl+K+J unfolds it recursively
- Ctrl+Shift+[ folds a section of code, Ctrl+Shift+] unfolds it

remember, Ctrl+K+S is the only keybind you really need.
