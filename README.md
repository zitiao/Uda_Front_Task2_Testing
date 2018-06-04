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
1. allFeeds 变量被声明。
2. allFeeds 中的每一项都必须同时包括name 和 url，且不为空。

### The menu
查看 `body` 的 `className`，为 `.menu-hidden` 时，则菜单隐藏。

1. 菜单默认隐藏。
2. jQuery 的 toggleClass 方法有效。

### loadFeed
异步接口，调用 `loadFeed` 方法获取页面内容。第一个参数 `id` 始终使用数字0。

1. 调用方法成功并有返回值（`.entry` 有内容 ）
2. 当调用方法获取内容时，`.entry` 有变更