# CLI-powermenu
Just a plain and simple terminal powermenu for Linux, written in Python with `ncurses` library, inspired by `ncmpcpp` command window.

![](https://github.com/Flock137/CLI-powermenu/blob/main/power.png)

## Instruction 
1. Create the directory `~/.local/bin` directory`
```
cd .local
mkdir bin
```

2. Copy the (raw text of) `powermenu` script in this repository, then:
```
vim ~/.local/bin/powermenu
# You can use other text editor that you prefer
```
Paste the script in that file

3. Type `chmod u+x ~/.local/bin/powermenu`
4. For the script to be used system-wide, instead of being able to only execute it while you were in the specific directory right above, you need to put it on PATH:
- If you use `bash` or/and `zsh` shell, paste in either `.bashrc` or/and `.zshrc`: `export PATH="$HOME/.local/bin:$PATH"`. Finally, exit, then re-enter the terminal.
- If you use `fish` shell, paste this line in `~/.config/fish/config.fish`: `set -gx PATH $HOME/.local/bin $PATH`. Then exit and re-enter the terminal.
