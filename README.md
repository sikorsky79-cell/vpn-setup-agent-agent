# vpn-build-agent

自建 VPN 搭建助手插件：先摸清用途与预算，再协助选择出口主机、部署抗干扰协议，并按设备交付订阅和流量提醒。

本插件只包含技能说明（`SKILL.md`），不含服务器地址、密钥或订阅链接，也不会在安装时执行远程代码。

## 包含的技能

| 技能 | 作用 |
|------|------|
| `vpn-getting-started` | 新导入后的第一次对话：一次只问一件事，摸底够用后再进入搭建流程。 |
| `vpn-build-flow` | 从云厂商选择到协议部署、订阅交付和流量护栏的标准流程。 |

## 目录

- `.grok-plugin/plugin.json` — 插件清单
- `skills/vpn-getting-started/SKILL.md` — 开场摸底
- `skills/vpn-build-flow/SKILL.md` — 搭建流程
- `LICENSE` — MIT 许可证
- `README.md` — 本说明

## 使用

在 Grok 插件市场安装本插件后，当用户提到自建 VPN、选主机、部署协议或交付订阅时，助手应先按 `vpn-getting-started` 摸底，再按 `vpn-build-flow` 执行。

硬约束（详见 `vpn-build-flow`）：月预算有硬顶；花钱、改防火墙、重启或换 IP 前必须征得用户同意；不要在对话里复述或写入任何私人服务器信息。

本插件不调用固定的网络接口，也不要求预置凭据。若搭建过程中需要打开云厂商网站或生成订阅，一律在用户本机会话中进行，并由用户确认。

## 版权

版权所有 © 2026 拨浪鼓（ORRA）

本项目以 [MIT License](./LICENSE) 发布。衍生作品须保留本版权声明。
