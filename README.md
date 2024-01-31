# tmux fastest cheat sheet
tmux is terminal multiplexer that allow you run multiple terminals inside terminal. here is the minimal cheat sheet that help you use tmux:
- [operation](#operation "goto operation")
- [configuration](#configuration "goto configuration")
### operation
command `tmux` launch a new tmux terminal session with one terminal window\
`Ctrl` + `B` then `:new` add a new tmux terminal session with one terminal window\
`Ctrl` + `B` then `D` detach tmux terminal session and go back to home terminal\
command `tmux a` attach terminal session back\
`Ctrl` + `B` then `S` list all terminal sessions; `H` `J` `K` `L` to navigate; `Enter` to enter in; `X` to kill; `Esc` go back\
\
`Ctrl` + `B` then `C` add a new terminal window\
`Ctrl` + `B` then `N` go next window\
`Ctrl` + `B` then `P` go previous window\
`Ctrl` + `B` then `W` list all terminal windows; `H` `J` `K` `L` to navigate; `Enter` to enter in; `X` to kill; `Esc` go back\
\
`Ctrl` + `B` then `%` add new terminal window pane horizontally\
`Ctrl` + `B` then `"` add new terminal window pane vertically\
`Ctrl` + `B` then ⬅️ ⬆️ ⬇️ ➡️ navigate activation to another pane\
`Ctrl` + `B` then `{` move current pane to left\
`Ctrl` + `B` then `}` move current pane to righr\
`Ctrl` + `B` then `Z` zoom in current pane to full screen or zoom out full screen\
`Ctrl` + `B` then `X` to kill current window or pane\

`Ctrl` + `B` then `T` show big clock; any key to exit clock
### configuration
systemwide config file `/etc/tmux.conf`\
user specific config file `~/.tmux.conf`\
\
command `tmux source-file /etc/tmux.conf` reload config file\

- - - -
Licence: [CC BY-SA](https://creativecommons.org/licenses/by-sa/4.0/)
