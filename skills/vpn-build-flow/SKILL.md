---
name: vpn-build-flow
description: Use when guiding a user through self-hosted anti-censorship VPN setup from cloud selection to subscription delivery and traffic guardrails.
---

# VPN 搭建标准流程

## 硬原则
- 月预算硬顶；双边流量计费按约一半估可用量。
- 出口优先家用宽带/住宅 IP（访问 AI 服务）；机房 IP 仅备选。
- 协议默认抗干扰：VLESS+REALITY@443 + Hysteria2 备线；禁烂大街 SNI；Hysteria2 禁橙云。
- 禁公网明文 HTTP 面板/订阅；一次性链接禁预览、禁可点击聊天投递。
- 改防火墙/SSH 前先有快照或控制台逃生。
- 注册前关代理；失败≤2次冷却；约48h换商。

## 步骤
0 摸底：用途、预算、预估流量、运营商城市、设备、客户端、境外卡/域名、可否换商。
0b 有效流量与档位换算。
1 厂商评分卡（注册/支付/UDP/流量规则/换IP/住宅出口/干净度）；淘汰注册不过、开不出、秒墙。
2 协助注册；失败查社区；时间盒换商；成功验开机+账单告警。
3 静态IP→双防火墙→运维钥→自动快照→再收端口（默认不开80）。
4 部署主备协议；多运营商 TCP/UDP 自检。
5 按端推荐客户端并生成对应格式订阅；附泄露重置说明。
6 客户端扣费与流量提示；近超额每5分钟刷新；云侧阶梯告警；动作需确认。
7 巡检/简报/备份与故障树交接。

花钱、改防火墙、重启、换IP前必须征得用户同意。
