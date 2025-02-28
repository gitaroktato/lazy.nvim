# 💤 LazyVim

A starter template for [LazyVim](https://github.com/LazyVim/LazyVim).
Refer to the [documentation](https://lazyvim.github.io/installation) to get started.

## Installation steps
```
git clone https://github.com/gitaroktato/lazy.nvim ~/.config/nvim
```

## What needs to be installed locally
```shell
pip install pyright ruff debugpy neovim
```

## Update `pyright`
`MasonInstall pyright@1.1.395`
- https://github.com/williamboman/mason.nvim/discussions/880

## To start with a specific `PYTHONPATH`
```shell
PYTHONPATH=`pwd`:$PYTHONPATH nvim .
```

## Fixing the `debugpy` issue
```shell
cd ~/.local/share/nvim/mason/packages
mkdir -p debugpy && cd debugpy
python -m venv venv
venv/bin/pip install debugpy
```
- https://github.com/microsoft/debugpy/issues/1345

## Hotkeys to remember
**Open up error logs**
`:mess` or `:Noice log`

**File explorer**
Open/close
`<SPACE>e`

Show/hide hidden
`H`

**Buffers - e.g. tabs**
`<SPACE>bb`
- https://www.reddit.com/r/neovim/comments/1bet4xt/how_to_switch_tabs_in_lazyvim/

**Navigating**
Move cursor in history
`ctrl+i, ctrl+o`
- https://www.reddit.com/r/neovim/comments/12kepcz/is_there_a_way_to_go_to_the_previous_cursor/

**Ruff, Python**
Getting errors
`<SPACE>cd`
- https://www.reddit.com/r/neovim/comments/13t74ut/how_can_i_get_better_looking_errors/

Comment out multiple lines
`gc`
- https://www.reddit.com/r/neovim/comments/1ejro2k/im_not_able_to_use_comment_multiple_line_feature/
  
Find references
`gr`

Outline
`<leader>cs`
- https://www.lazyvim.org/keymaps#outlinenvim

### LazyGit
- https://github.com/jesseduffield/lazygit/blob/master/docs/keybindings/Keybindings_en.md

## References and Guides:
- https://www.reddit.com/r/neovim/comments/1fgq6rq/lazyvim_python_debug_setup/
- https://lazyvim-ambitious-devs.phillips.codes/course
