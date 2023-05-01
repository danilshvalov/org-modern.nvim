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

![Screenshot 2023-05-01 at 23 57 55](https://user-images.githubusercontent.com/57654917/235530013-125c4108-1354-4871-9423-2520975ab866.png)
