# virt-column.nvim

Display a character as the colorcolumn.

## Difference between the original [virt-column](https://github.com/IronGeek/virt-column.nvim) and this virt-column

- Fix the virtual line would display even at index < 0.
  (Fix a visual bug on horizontal scroll)
- Extend the virtual line to the whole visual space.
- Above feature works on multiple columns. (fix from [another fork](https://github.com/FY0u11/virt-column.nvim/))

## Install

For [lazy.nvim](https://github.com/folke/lazy.nvim):
Create a .lua file in ~/.config/nvim/lua/plugins/ and apply below content

```lua
return {
  {
    "1lazyl/virt-column.nvim",
    ---@module "virt-column"
    ---@type virtcolumn.config
    opts = {
      enabled = true,

      -- for multiple columns with different characters, use ["|", "│"]
      char = "│",

      -- comma separated list of column numbers where vertical lines appear
      virtcolumn = "100,120",

      -- table of highlight group names to style each vertical line
      highlight = { "VirtColumn", "VirtColumn2" },
    },
    lazy = true,
    event = "VeryLazy",
  },
}
```

