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

<img width="1440" alt="Screenshot 2023-05-01 at 18 45 15" src="https://user-images.githubusercontent.com/57654917/235480782-dcb6b607-73f0-4882-a882-1d4e05015997.png">
