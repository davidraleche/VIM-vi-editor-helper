# VIM-helper

https://devhints.io/vim

https://vim.rtorr.com/


### vi command 	description
0 	move to beginning of the current line
$ 	move to end of line
H 	move to the top of the current window (high)
M 	move to the middle of the current window (middle)
L 	move to the bottom line of the current window (low)
1G 	move to the first line of the file
20G 	move to the 20th line of the file
G 	move to the last line of the file

### SAVE QUIT
    :wq or :x or ZZ - write (save) and quit

### GO TO LINE
    :n 	Go to line n
    nG 	Go to line n

### COPY
    yy - yank (copy) a line
    2yy - yank (copy) 2 lines
    yw - yank (copy) the characters of the word from the cursor position to the start of the next word
    y$ - yank (copy) to end of line
   

### Paste
    
    p - put (paste) the clipboard after cursor
    P - put (paste) before cursor
    

### DELETE    
    dd - delete (cut) a line
    2dd - delete (cut) 2 lines
    dw - delete (cut) the characters of the word from the cursor position to the start of the next word
    D - delete (cut) to the end of the line
    d$ - delete (cut) to the end of the line
    x - delete (cut) character
    
    
###  Cursor movement

    h - move cursor left
    j - move cursor down
    k - move cursor up
    l - move cursor right
    H - move to top of screen
    M - move to middle of screen
    L - move to bottom of screen
    w - jump forwards to the start of a word
    
    
### Working with multiple files

    :e file - edit a file in a new buffer
    :bnext or :bn - go to the next buffer
    :bprev or :bp - go to the previous buffer
    :bd - delete a buffer (close a file)
    :ls - list all open buffers
    :sp file - open a file in a new buffer and split window
    :vsp file - open a file in a new buffer and vertically split window
    Ctrl + ws - split window
    Ctrl + ww - switch windows
    Ctrl + wq - quit a window
    Ctrl + wv - split window vertically
    Ctrl + wh - move cursor to the left window (vertical split)
    Ctrl + wl - move cursor to the right window (vertical split)
    Ctrl + wj - move cursor to the window below (horizontal split)
    Ctrl + wk - move cursor to the window above (horizontal split)
    
    
    
### Search and replace

    /pattern - search for pattern
    ?pattern - search backward for pattern
    \vpattern - 'very magic' pattern: non-alphanumeric characters are interpreted as special regex symbols (no escaping needed)
    n - repeat search in same direction
    N - repeat search in opposite direction
    :%s/old/new/g - replace all old with new throughout file
    :%s/old/new/gc - replace all old with new throughout file with confirmations
    :noh - remove highlighting of search matches


### Search in multiple files

    :vimgrep /pattern/ {file} - search for pattern in multiple files

e.g.:vimgrep /foo/ **/*

    :cn - jump to the next match
    :cp - jump to the previous match
    :copen - open a window containing the list of matches
