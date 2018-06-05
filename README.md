# 简述
共包含 8 个测试内容
1. RSS Feeds
- are defined
- url should be defined and not empty
- name should be defined and not empty
2. The menu
- should hide at default
- should display at first click
- should hide at another click
3. Initial Entries
- should be called and have at least one element
4. New Feed Selection
- should change the content when new feed added

### RSS Feeds
1. `1allFeeds` 变量被声明。
2. `allFeeds` 中的每一项都必须同时包括`name` 和 `url`，且不为空。
3. `url`的格式必须正确。

### The menu
<!-- 查看 `body` 的 `className`，为 `.menu-hidden` 时，则菜单隐藏。 -->
查看 `body` 的 `className`，包含 `.menu-hidden` 时，则菜单隐藏。
1. 菜单默认隐藏。
2. `jQuery` 的 `toggleClass` 方法有效。
3. `jQuery` 的 `hasClass` 方法。

### loadFeed
异步接口，调用 `loadFeed` 方法获取页面内容。第一个参数 `id` 始终使用数字0。

1. 调用方法成功并有返回值（`.entry` 有内容 ）。
2. 当调用方法获取内容时，`.entry` 有变更(检查的是内容，而不是条目，之前没发现，条目不是新增的方式，而是覆盖)。