# 💤 LazyVim

A starter template for [LazyVim](https://github.com/LazyVim/LazyVim).
Refer to the [documentation](https://lazyvim.github.io/installation) to get started.

## Installation steps
```
git clone https://github.com/gitaroktato/lazy.nvim ~/.config/nvim
```

# Meta key binding
`<M-` options have to set `alt_send_esc: false`
- https://github.com/alacritty/alacritty/issues/4048
- https://github.com/alacritty/alacritty/issues/4557
- https://stackoverflow.com/questions/11876485/how-to-disable-generating-special-characters-when-pressing-the-alta-optiona

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

**Breakpoints in library code**
`:DapShowLog` to view logs
Setting the `justMyCode = false` variable
- https://github.com/mfussenegger/nvim-dap/discussions/927
- https://github.com/mfussenegger/nvim-dap/discussions/846
- https://github.com/nvim-neotest/neotest/issues/460
- https://www.reddit.com/r/neovim/comments/1awity5/setting_up_nvimdap_dappython_for_debugging_python/

## Hotkeys to remember
**Open up error logs**
`:mess` or `:Noice log`

**File explorer**
Open/close
`<SPACE>e`

Show/hide hidden
`H`

Show/hide ignored in .gitignore
`I`

**Buffers - e.g. tabs**
`<SPACE>bb`
- https://www.reddit.com/r/neovim/comments/1bet4xt/how_to_switch_tabs_in_lazyvim/

**Navigating**
Move cursor in history
`ctrl+i, ctrl+o`
- https://www.reddit.com/r/neovim/comments/12kepcz/is_there_a_way_to_go_to_the_previous_cursor/

Word wrap
`<space>uw`
- https://github.com/LazyVim/LazyVim/discussions/1959

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

## Explorer Snack
- https://github.com/folke/snacks.nvim/blob/main/docs/picker.md

### LazyGit
- https://github.com/jesseduffield/lazygit/blob/master/docs/keybindings/Keybindings_en.md

## References and Guides:
- https://www.reddit.com/r/neovim/comments/1fgq6rq/lazyvim_python_debug_setup/
- https://lazyvim-ambitious-devs.phillips.codes/course
