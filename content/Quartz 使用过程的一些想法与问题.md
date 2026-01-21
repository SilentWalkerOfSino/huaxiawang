# Quartz 使用过程的一些想法与问题

## 主页布局设计
quartz 中页面布局设计，可以使用插件快捷的添加固定页面布局。
使用 ContentIndex 插件（推荐）
在 quartz.layout.ts 的布局中加入 ContentIndex 组件：
```
// quartz.layout.ts
import ContentIndex from "./components/ContentIndex"
```


## 问题

主页中的配置
注意这里对于 YAML 格式的配置，比如这里的在 `---`包裹的部分，属于是 key-value 式的配置项，必须是 `key: value`的格式，且在`:`后面必须有空格。

```
---
title: 欢迎来到华夏王的主页
---
```

Front Matter 使用的是 YAML 语言。
