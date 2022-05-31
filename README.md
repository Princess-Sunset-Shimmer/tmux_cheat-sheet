# tmux_cheat-sheet
a simple cheat sheet help new comers to use tmux
```
tmux
|
+-- session command
|   |
|   +-- tmux  // create session
|   |
|   +-- tmux list-session  // tmux ls
|   |
|   +-- tmux attach  // tmux a; attach session
|   |
|   +-- tmux attach -t name  // tmux a -t name; attach target session
|
+-- operation
    |
    +-- prefix
    |   |
    |   +-- ctrl + b  // entry prefix
    |   |
    |   +-- ctrl + d  // delete pane
    |
    +-- subfix
        |
        +-- session
        |   |
        |   +-- s  // session panel
        |   |
        |   +-- d  // disconnect session
        |   |
        |   +-- $  // rename session
        |
        +-- window
        |   |
        |   +-- create
        |   |   |
        |   |   +-- c  // create new window
        |   |   |
        |   |   +-- &  // kill window
        |   |   |
        |   |   +-- ,  // rename window
        |   |
        |   +-- navigate
        |       |
        |       +-- p  // previous window
        |       |
        |       +-- n  // next window
        |
        +-- pane
            |
            +-- split
            |   |
            |   +-- %  // split vertical
            |   |
            |   +-- "  // split horizontal
            |
            +-- navigate
                |
                +-- left, down, up, right
                    |
                    +-- left, down, up, right
```
