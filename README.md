# Clash Meta 订阅转换模板

自维护版 subconverter 配置，基于 [usbog232/clashmetadingyue](https://github.com/usbog232/clashmetadingyue) 的 `new-meta.ini`。

## 相对原版的改动

| 项 | 说明 |
|---|---|
| `🧊 冷门节点` | 由 `select` 改为 `url-test`，自动测速选优（间隔 300s，容差 50ms） |

## 使用

在 subconverter / 订阅转换里把「远程配置」指到本仓库的 raw 地址，例如：

```text
https://raw.githubusercontent.com/<你的用户名>/<仓库名>/main/new-meta.ini
```

或 jsDelivr：

```text
https://cdn.jsdelivr.net/gh/<你的用户名>/<仓库名>@main/new-meta.ini
```

## 文件

- `new-meta.ini` — 主模板（规则 + 策略组）
