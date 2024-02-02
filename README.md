# tmux fastest cheat sheet
tmux is terminal multiplexer that allow you run multiple terminals inside terminal. here is the minimal cheat sheet that help you use tmux:
- [operation](#operation "goto operation")
- [configuration](#configuration "goto configuration")
### operation
command `tmux` launch a new tmux terminal session with one terminal window\
`Ctrl` + `B` then `:new` add a new tmux terminal session with one terminal window\
`Ctrl` + `B` then `D` detach tmux terminal session and go back to home terminal\
command `tmux a` attach terminal session back\
`Ctrl` + `B` then `S` list all terminal Sessions and Windows; `H` `J` `K` `L` to navigate; `Enter` to enter in; `X` to kill; `Esc` go back\
\
`Ctrl` + `B` then `C` add a new terminal window\
`Ctrl` + `B` then `N` go next window\
`Ctrl` + `B` then `P` go previous window\
`Ctrl` + `B` then `X` to kill current window or pane\
\
`Ctrl` + `B` then `%` add new terminal window pane horizontally\
`Ctrl` + `B` then `"` add new terminal window pane vertically\
`Ctrl` + `B` then ⬅️ ⬆️ ⬇️ ➡️ navigate activation to another pane\
`Ctrl` + `B` then `{` move current pane to left\
`Ctrl` + `B` then `}` move current pane to righr\
`Ctrl` + `B` then `Z` zoom current pane to full screen or unzoom\
`Ctrl` + `B` then `:resize-pane -L 1` resize pane 1 unit more to Left\
`Ctrl` + `B` then `:resize-pane -D 1` resize pane 1 unit more to Down\
`Ctrl` + `B` then `:resize-pane -U 1` resize pane 1 unit more to Up\
`Ctrl` + `B` then `:resize-pane -R 1` resize pane 1 unit more to Right\
\
`Ctrl` + `B` then `T` show big clock; any key to exit clock
### configuration
systemwide config file: `/etc/tmux.conf`\
user specific config file: `~/.tmux.conf`\
\
command `tmux source-file /etc/tmux.conf` reload config file\
\
`set -g pane-border-status top` add status border to top of pane\
`set -g pane-border-status bottom` add status border to bottom of pane\
`set -g pane-border-style fg=brightcyan` set pane border color, `bg=green,fg=cyan` set both background and foreground color\
`set -g pane-active-border-style fg=white` set active pane border color, `bg=blue,fg=yellow` set both background and foreground color\
`set -g pane-border-format "#[fg=red]<#P>#[fg=green]#{pane_current_path}>"` set contents of pane status border, `""` clear contents\
\
`set -g status-position top` move status bar to top\
`set -g status-style bg=black` set tatus bar color, `bg=black,fg=brightblue` set both background and foregound color\
`set -g status-justify centre` move window list to centre\
`set -g window-status-current-format "#{?window_zoomed_flag,( #I ),(#I)}"` set contents of current window in window list\
`set -g window-status-format " #I "` set contnets of other windows in window list\
`set -g status-right "#[fg=cyan]%I:%M %p "` set contents of status bar right side\
`set -g status-left "[#S]"` set contents of status bar left side\
\
`set -g message-status bg=black,fg=white` set message bar colors
| tmux replacement   | means                        |
| ------------------ | ---------------------------- |
| `#(shell-command)` | first line of command output |
| `#[attributes]`    | change Colors or Attributes  |
| `#H`               | full Hostname                |
| `#h`               | short hostname               |

- - - -
Licence: [CC BY-SA](https://creativecommons.org/licenses/by-sa/4.0/)
