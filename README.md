# meta-check

自维护 Clash Meta 订阅转换模板（**29 策略组 + 8 节点组**）。

## 远程配置

```text
https://raw.githubusercontent.com/cub4libre/meta-check/main/new-meta.ini
```

内含 `clash_rule_base` → `base-meta.yaml`（国内 DNS / respect-rules / TUN / 嗅探）。

## 节点组（8）

| 组 | 作用 |
|---|---|
| `🧭 手动选择` | `select` 全节点，**可固定到某一个节点** |
| `♻️ 自动选择` | 全节点 url-test |
| `🇭🇰 HK` `🇹🇼 TW` `🇯🇵 JP` `🇸🇬 SG` `🇺🇸 US` | 地区 url-test |
| `🧊 冷门节点` | 非五区 url-test |

各应用策略组都挂了 `🧭 手动选择`，需要钉死单节点时选它即可。

## 策略组（29）

腾讯会议、国内应用、Apple、AI、Telegram、即时通讯、社交媒体、YouTube、Netflix、TikTok、Instagram、X、GitHub、测速工具、Steam、OKX、Binance、Bybit、加密货币、TradingView、Google、cloudflare、Microsoft、🚀手动选择、Default、漏网之鱼、SSH/RDP、非标端口、遵循规则。

## 上传 GitHub 时请包含

- `new-meta.ini`
- `base-meta.yaml`
- `rules/cn-apps.yaml`（抖音/快手/小红书，不依赖 GeoSite 的 douyin 条目）
- `rules/ssh-rdp-ports.yaml`
- `rules/tencent-meeting.yaml`
- `rules/tradingview.yaml`
