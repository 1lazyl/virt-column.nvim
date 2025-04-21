# 🚸 Notice

This branch is:

1. A fork of the original [virt-column.nvim](https://github.com/lukas-reineke/virt-column.nvim) + additional
   changes from the other branches not yet merged to upstream.

2. **Rebased** with upstream and **force-pushed** whenever new changes
   are introduced in the other branches.

3. Expected to have conflicts and cause headaches when pulled or fetched.

4. **AS IS**, use it at your own risk, [here be dragons](https://en.wikipedia.org/wiki/Here_be_dragons).

---

# virt-column.nvim

Display a character as the colorcolumn.

<img width="900" src="https://user-images.githubusercontent.com/12900252/143544703-d94d6e9e-75f8-407d-976e-0fd5b341d751.png" alt="Screenshot" />

## Install

Use your favourite plugin manager to install.

For [lazy.nvim](https://github.com/folke/lazy.nvim):

```lua
{ "lukas-reineke/virt-column.nvim", opts = {} },
```

For [pckr.nvim](https://github.com/lewis6991/pckr.nvim):

```lua
use "lukas-reineke/virt-column.nvim"
```

## Setup

To configure virt-column.nvim you need to run the setup function.

```lua
require("virt-column").setup()
```

Please see `:help virt-column.txt` for more details and all possible values.

## Thanks

Thank you @francium for the idea.
