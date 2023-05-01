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

![Screenshot 2023-05-01 at 23 59 08](https://user-images.githubusercontent.com/57654917/235530277-94bbd233-4030-4fe5-83bd-91c0f133bd00.png)
