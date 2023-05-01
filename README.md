## Modern menu

```lua
local Menu = require("org-modern.menu")

require("orgmode").setup({
  ui = {
    menu = {
      handler = function(title, items)
        Menu:new({
          window = {
            margin = { 1, 0, 1, 0 },
            padding = { 0, 1, 0, 1 },
            title_pos = "center",
            border = "single",
            zindex = 1000,
          },
          icons = {
            separator = "➜",
          },
        }):open(title, items)
      end,
    },
  },
})
```
