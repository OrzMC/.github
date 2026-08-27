<div align="center">

<img src="https://raw.githubusercontent.com/OrzMC/.github/main/assets/OrzMC.png" width="140" alt="OrzMC logo">

# 🇨🇳 OrzMC

围绕 PaperMC 生态的 Minecraft 社区服务器开源运维组织——自研插件、CLI 与运维工具，面向**玩家**与**开发者**开放。

[🌐 官网](https://orzmc.jokerhub.cn) · [Modrinth](https://modrinth.com/organization/orzmc) · [Hangar](https://hangar.papermc.io/wangzhizhou666) · [𝕏 @OrzMC666](https://x.com/OrzMC666)

[![GitHub Stars](https://img.shields.io/github/stars/OrzMC/OrzMC?style=flat-square&label=GitHub%20Stars&color=blue)](https://github.com/OrzMC/OrzMC)
![PaperMC](https://img.shields.io/badge/PaperMC-1.13%2B-FAAE2A?style=flat-square)
![license](https://img.shields.io/badge/license-Apache--2.0%20%7C%20MIT%20%7C%20GPL--3.0-blue?style=flat-square)
![Java](https://img.shields.io/badge/Java-21-orange?style=flat-square)
[![PyPI](https://img.shields.io/pypi/v/orzmc-app?style=flat-square&label=PyPI)](https://pypi.org/project/orzmc-app/)

</div>

## 🧩 组件生态

```
玩家端      OrzMCApp (macOS/iOS) · OrzWebMC (浏览器)
  ▼ 连接
网络层      OrzMCProxy —— FRP 三网中转，解决跨运营商延迟/拒连
  ▼
服务器核心  PaperMC 1.13+ + OrzMCPlugin（白名单 / 机器人 / 指令）
  ▼ 运维
运维部署    orzmc-app CLI · OrzMCAdmin · OrzMCDeploy · OrzMCBackup · rust-thanos
  ▼
站点社区    OrzMCSite（官方网站）
```

<details>
<summary>📦 全部项目 · 语言 / 许可 / 获取</summary>

| 分类 | 项目 | 一句话说明 | 语言 | 许可 | 获取 |
|---|---|---|---|---|---|
| 主仓库 | **OrzMC** | All-in-One Super Repo，15 个子模块的总入口 | Shell | Apache-2.0 | [GitHub](https://github.com/OrzMC/OrzMC) |
| 插件 | **OrzMCPlugin** | 服务器核心管理插件：白名单、机器人、`/tpbow` `/guide` `/bot` `/portal` `/menu`、TNT 防护、区域限制、跨服传送门 | Java | GPL-3.0 | [Hangar](https://hangar.papermc.io/wangzhizhou666) |
| 插件 | LoginSecurity | 登录认证插件 | Java | Apache-2.0 | [repo](https://github.com/OrzMC/LoginSecurity) |
| 插件 | GetMeHome | `/home` 家的传送插件 | Java | MIT | [repo](https://github.com/OrzMC/GetMeHome) |
| 插件 | DeathChest | 死亡掉落箱子插件 | Java | MIT | [repo](https://github.com/OrzMC/death-chest) |
| 插件 | EzShops | 商店插件 | Java | MIT | [repo](https://github.com/OrzMC/EzShops) |
| CLI/工具 | **orzmc-app** | 跨平台 CLI：客户端启动 / 服务端一键部署 | Python | Apache-2.0 | [PyPI](https://pypi.org/project/orzmc-app/) |
| CLI/工具 | **OrzMCAdmin** | 服主自动化运维，可交给 AI Agent | Python | MIT | [repo](https://github.com/OrzMC/OrzMCAdmin) |
| CLI/工具 | **OrzMCBackup** | MCA 世界备份 / 优化，按 InhabitedTime 清理区块 | Kotlin | © 2026 wangzhizhou | [repo](https://github.com/OrzMC/OrzMCBackup) |
| CLI/工具 | rust-thanos | Rust 版区块清理工具 | Rust | [占位] | [repo](https://github.com/OrzMC/rust-thanos) |
| CLI/工具 | thanos | PHP 版区块清理工具（上游 fork） | PHP | MIT | [repo](https://github.com/aternosorg/thanos) |
| 部署/网络 | **OrzMCDeploy** | Docker 部署：MCSManager / EasyBot / MariaDB / Gatus | Shell | [占位] | [repo](https://github.com/OrzMC/OrzMCDeploy) |
| 部署/网络 | **OrzMCProxy** | FRP 跨网中转，解决三网延迟 / 拒连 | Shell | [占位] | [repo](https://github.com/OrzMC/OrzMCProxy) |
| 客户端/应用 | **OrzMCApp** | macOS/iOS 应用 + Swift 库 | Swift | [占位] | [repo](https://github.com/OrzMC/OrzMCApp) |
| 客户端/应用 | OrzWebMC | 浏览器玩 Minecraft 的探索 | Shell | [占位] | [repo](https://github.com/OrzMC/OrzWebMC) |
| 站点/社区 | **OrzMCSite** | 官方网站 orzmc.jokerhub.cn | HTML | [占位] | [官网](https://orzmc.jokerhub.cn) |
| 运维脚本 | scripts/ · skins/ | 运维脚本 / 玩家皮肤 | Shell | — | 见 [OrzMC](https://github.com/OrzMC/OrzMC) |

</details>

## 🎮 玩家 · 👨💻 开发者

**玩家进服**：申请白名单 → 审核通过 → 进服（审核制）。服务器地址、版本与社群入口见 [官网](https://orzmc.jokerhub.cn)。

**开发者贡献**：从 [OrzMC](https://github.com/OrzMC/OrzMC) 开始，fork → PR。技术栈 Java / Kotlin / Rust / Python / Swift / Shell。新手看各仓库 `good first issue`。

## 💖 支持我们

核心功能永久免费，捐赠与返佣全部用于覆盖服务器与开发成本，资金去向公开透明。

[❤️ 爱发电捐赠](https://ifdian.net/a/orzmc) · [☁️ 腾讯云返佣](https://curl.qcloud.com/yc9gf7MY) · [☁️ 阿里云返佣](https://www.aliyun.com/product/ecs?userCode=uqebe1h3)

> 🚀 增值功能 · 🛠️ 代运维服务 —— 筹备中

---

遵循 Mojang EULA · 与 Mojang / Microsoft 无关
