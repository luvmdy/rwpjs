---
nav:
  title: 文档
  path: /introduce
group:
  path: /introduce
  title: RWP.JS
order: 2
---

# 约定路由

我们约定项目中至少含有以下目录 `src/pages/*`

```
src
└─pages
    ├─.rwp
    └─demo
    | └─demo.route.tsx
    └─hello.route.tsx
    └─index.route.tsx
```

> 所有以 `*.route.tsx` 结尾的文件,才会自动注册为路由信息。

例如以上的三个文件夹，那么对应的路由信息则为

- /demo/demo
- /hello
- /

`src/pages/index.route.tsx` 表示首页信息

## 关于 layout

主框架代码则是加载`src/layouts/index.tsx`, 如果当前目录下拥有`layout.tsx`则会作为嵌套路由的布局信息



