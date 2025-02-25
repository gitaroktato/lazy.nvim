# 💤 LazyVim

A starter template for [LazyVim](https://github.com/LazyVim/LazyVim).
Refer to the [documentation](https://lazyvim.github.io/installation) to get started.

## What needs to be installed locally
```shell
pip install pyright ruff debugpy
```

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
```
<SPACE>bb
```
- https://www.reddit.com/r/neovim/comments/1bet4xt/how_to_switch_tabs_in_lazyvim/

**Ruff, Python**
Getting errors
```
<SPACE>cd
```
- https://www.reddit.com/r/neovim/comments/13t74ut/how_can_i_get_better_looking_errors/

Comment out multiple lines
```
gc
```
- https://www.reddit.com/r/neovim/comments/1ejro2k/im_not_able_to_use_comment_multiple_line_feature/

## References and Guides:
- https://www.reddit.com/r/neovim/comments/1fgq6rq/lazyvim_python_debug_setup/
- https://lazyvim-ambitious-devs.phillips.codes/course
