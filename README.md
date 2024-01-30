# tmux fastest cheat sheet
tmux is terminal multiplexer that allow you run multiple terminals inside terminal. here is the minimal cheat sheet that help you use tmux:
- [operation](#operation "goto operation")
- [configuration](#configuration "goto configuration")
### operation
command `tmux` launch a new tmux terminal session with one terminal window\
`Ctrl` + `B` then `D` detach tmux terminal session and go back to home terminal\
command `tmux a` attach terminal session\
`Ctrl` + `B` then `W` list all terminal sessions; `H` `J` `K` `L` to navigate; `Enter` to enter in; `X` to kill\
\
`Ctrl` + `B` then `%` add new terminal window pane horizontally\
`Ctrl` + `B` then `"` add new terminal window pane vertically\
`Ctrl` + `B` then ⬅️ ⬆️ ⬇️ ➡️ navigate activation to another pane\
`Ctrl` + `B` then `{` move current pane to left\
`Ctrl` + `B` then `}` move current pane to righr\
`Ctrl` + `B` then `Z` zoom in current pane to full screen or zoom out full screen\
`Ctrl` + `B` then `X` to kill current window pane
### configuration
systemwide config file `/etc/tmux.conf`\
user specific config file `~/.tmux.conf`\
\
command `tmux source-file /etc/tmux.conf` reload config file\
- - - -
Licence: [CC BY-SA](https://creativecommons.org/licenses/by-sa/4.0/)
