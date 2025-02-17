# Setup-tool

# VS Code Ubuntu
+ Always ask for Permission:
=> (Link)[https://dev.to/rahedmir/visual-studio-code-always-ask-for-permission-to-save-files-in-linux-140p]


# Tmux Setup:
** (Installation Document)[https://github.com/tmux/tmux/wiki/Installing] **
    - `sudo apt install tmux`
+ (Tmux CPU Memory Monitor Plugin)[https://github.com/hendrikmi/tmux-cpu-mem-monitor]
+ (Tutorial)[https://www.youtube.com/watch?v=adsnH--SAww]
+ Create Configuration files:
`mkdir -p .config/tmux`
`touch .config/tmux/tmux.conf`
# Tmux Syntax:
+ Create new session: `tmux new -s <name of session>`
+ Detach from a Tmux Session: `Ctrl + B` then press d
+ Create new windows in a sessions: `Ctrl + B` then press c
+ Rename Windows: `Ctrl + B` then press ,
+ Switching betwwen windows: `Ctrl + B` then press p to the previous tabs, and n to the next tabs
+ Split windows vertically: `Ctrl + B` then % (shift + 5)
+ Enter the commands mode of Tmux: `Ctrl + B` then press : (shift + ;) - type list-keys to shows all binding keys.

# Nvim SetUp Ubuntu:
** Latest Nvim Set up (Pre-built Archives) **:
`curl -LO https://github.com/neovim/neovim/releases/latest/download/nvim-linux-x86_64.tar.gz`
`sudo rm -rf /opt/nvim`
`sudo tar -C /opt -xzf nvim-linux-x86_64.tar.gz`
+ Adding env path to shell config (~/.bashrc, ~/.zshrc, ...):
`export PATH="$PATH:/opt/nvim-linux-x86_64/bin"`
** Latest Nvim Set up (Snap) **:
`sudo snap install nvim --classic`
** (Tutorials)[https://www.youtube.com/watch?v=KYDG3AHgYEs] **
+ Plugin: (KickStart)[https://github.com/nvim-lua/kickstart.nvim]
Basic:
`sudo apt install neovim`
`mkdir -p .config/nvim`
`cd .config/nvim`
`touch init.lua`
`mkdir lua`
`touch options.lua`
Advance:
`git clone https://github.com/nvim-lua/kickstart.nvim.git "${XDG_CONFIG_HOME:-$HOME/.config}"/nvim`
``
``
``
``
``
``
``
``
``
``


# Nvim syntax
+ 0 : return to the beginning of the string
+ c + shift + G : copy and delete the string (let the cursor in the beginning of the string- use this in normal mode )
+ x : delete charater (after the cursor then before the cursor then the charater in the cursor - use in normal mode)
+ d : delete row
+ g : got to the first charater
+ G (Shift + g) : go to the last charater
+ j : in NORMAL and VISUAL mode switching between lines
+ shift + j : in NORMAL mode delete each row, in VISUAL mode delete all rows selected
+ d : in NORMAL mode delete row in VISUAL mode delete all selected rows
+ shift + d : in VISUAL mode delete all selected rows  