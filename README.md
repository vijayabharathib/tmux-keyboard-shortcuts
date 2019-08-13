# Tmux Keyboard Shortcuts

List of frequently used Tmux keyboard shortcuts and commands. 

Manual from `man tmux` and/or `Prefix + ?` should server as good starting point. **`Prefix`** is `Ctrl + b` by default.

## Session Management

**Operation** | **Command / Key**
--------------|------------------
`tmux` | Create new session 
`Prefix + d` | Detach from a session
`tmux a -t <n>` | Attach to existing session (use auto generated number to target)
`tmux new -s <name>` | Create new session with given name
`tmux a -t <fuzzy name>` | Attach to existing session based on name
`tmux ls` | List available sessions
`Prefix + s` | Interactively attach to listed session
`Prefix + $` | Rename current session

## Window Management

**Operation** | **Command / Key**
--------------|------------------
`Prefix + c`| Create a new window within current session
`Prefix + w` | Interactively select the window
`Prefix + ,` | Rename current window
`Prefix + <n>` | Select the window at index given at `n`
`Prefix + '` | Key in window index to select the window
`Prefix + n` | Move to the next window
`Prefix + p` | Move to the previous window
`tmux movew -t<n>` | Move current window to specified index
`Prefix + l` | Last active window
`Prefix + f` | Find window by text content
`Prefix + &` | Kill window along with panes

## Pane Management 

**Operation** | **Command / Key**
--------------|------------------
`Prefix + %`| Split into vertical panes
`Prefix + "` | Split into horizontal panes
`Prefix + <arrow>` | Move to the pane in the direction of the arrow
`Prefix + o` | Cycle through the panes
`Prefix + Ctrl + <arrow>` | Resize pane by 1 row/col
`Prefix + Alt + <arrow>` | Resize pane by 5 rows/cols
`Prefix + x` | Kill pane
`Prefix + space` | Cycle between predefined layouts
`Prefix + z` | Toggle fullscreen for the pane

## Copy Mode

**Operation** | **Command / Key**
--------------|------------------
`Prefix + [` | Enter into copy/scroll mode
`q` | To exit out of copy/scroll mode
`Ctrl + Space` | Mark start of copy region
`<arrow>` | Navigate with arrow to select a region of text
`Alt + w` | Copy selected region
`Prefix + ]` | Paste copied text

## Credits
This collection is the result of several resources that helped me When I started with tmux. Some of them helped me solve a tmux problem. They might help you too.
* [The Tao of tmux](https://leanpub.com/the-tao-of-tmux/read) - A very useful book on tmux free to read online.
* A list of [keys from coderwall](https://coderwall.com/p/mxzdrg/keyboard-shortcuts-i-use-every-day-in-tmux)
* [A crash course from thoughtbot](https://robots.thoughtbot.com/a-tmux-crash-course)
* `Prefix + ?` from within tmux to list shortcuts keys!
* finally `man tmux` itself :-)
