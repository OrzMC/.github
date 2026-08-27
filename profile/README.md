<div align="center">

<img src="https://raw.githubusercontent.com/OrzMC/.github/main/assets/OrzMC.png" width="160" alt="OrzMC logo">

# 🇨🇳 OrzMC · PaperMC 社区服 · 开源运维与开发组织

一个长期运营的中文 Minecraft 社区服务器背后的 GitHub 组织——**自研插件、CLI 与运维工具**，面向**玩家**（进服 / 白名单）与**开发者**（贡献 / 自研）同时开放。

[🌐 官网](https://orzmc.jokerhub.cn) · [Modrinth](https://modrinth.com/organization/orzmc) · [Hangar](https://hangar.papermc.io/wangzhizhou666) · [𝕏 @OrzMC666](https://x.com/OrzMC666)

[![官网](https://img.shields.io/badge/官网-orzmc.jokerhub.cn-4F9DE0?style=flat-square)](https://orzmc.jokerhub.cn)
[![GitHub Stars](https://img.shields.io/github/stars/OrzMC/OrzMC?style=flat-square&label=GitHub%20Stars&color=blue)](https://github.com/OrzMC/OrzMC)
![PaperMC](https://img.shields.io/badge/PaperMC-1.13%2B-FAAE2A?style=flat-square)
![license](https://img.shields.io/badge/license-Apache--2.0%20%7C%20MIT%20%7C%20GPL--3.0-blue?style=flat-square)
![Java](https://img.shields.io/badge/Java-21-orange?style=flat-square)
[![PyPI](https://img.shields.io/pypi/v/orzmc-app?style=flat-square&label=PyPI)](https://pypi.org/project/orzmc-app/)

</div>

---

## 🎯 我们做什么

> **使命**：用开源的方式，长期维护一个稳定、开放、以社区为本的 PaperMC 服务器，并把过程中的代码、工具与经验沉淀下来，回馈 Minecraft 生态。

**我们做什么**
- 自研服务器插件与运维工具链（插件 / CLI / 部署 / 网络 / 应用 / 站点）
- 运营一个**审核制白名单**的中文社区服（国内 / 海外双服，隔离地图）
- 把运维经验沉淀为可复用的开源项目，欢迎 PR 与复用

**为什么值得关注**
- **玩家**：稳定、干净、遵守 Mojang EULA 的社区服，白名单审核进服
- **开发者**：Java / Kotlin / Rust / Python / Swift / Shell 全栈 Minecraft 项目矩阵
- **组织**：混合自营利模式（捐赠 + 增值 + 服务），长期可持续，而非「用爱发电」到停摆

## 🧩 组件生态与架构

从玩家端、网络层到服务器核心、运维站点，OrzMC 把整个社区服的每一层都做成了开源项目：

```
玩家端      OrzMCApp (macOS/iOS) · OrzWebMC (浏览器)
  │ 连接
网络层      OrzMCProxy —— FRP 三网中转，解决跨运营商延迟/拒连
  ▼
服务器核心  PaperMC 1.13+ + OrzMCPlugin（白名单 / 机器人 / 指令）
  │ 挂载
工具插件    LoginSecurity · GetMeHome · DeathChest · EzShops
  │ 运维
运维部署    orzmc-app CLI · OrzMCAdmin · OrzMCDeploy · OrzMCBackup · rust-thanos
  ▼
站点社区    OrzMCSite 官网 · Modrinth · Hangar · QQ / Discord
```

| 分类 | 项目 | 一句话说明 | 语言 | 许可 | 获取 |
|---|---|---|---|---|---|
| 主仓库 | **OrzMC** | All-in-One Super Repo，15 个子模块的总入口 | Shell | Apache-2.0 | [GitHub](https://github.com/OrzMC/OrzMC) |
| 插件 | **OrzMCPlugin** | 服务器核心管理插件：白名单管理、QQ / Discord / 飞书机器人、`/tpbow` `/guide` `/bot` `/portal` `/menu`、TNT 防护、区域限制、跨服传送门 | Java | GPL-3.0 | [Hangar](https://hangar.papermc.io/wangzhizhou666) |
| 插件 | LoginSecurity | 登录认证插件 | Java | [占位] | [repo](https://github.com/OrzMC/LoginSecurity) |
| 插件 | GetMeHome | `/home` 家的传送插件 | Java | MIT | [repo](https://github.com/OrzMC/GetMeHome) |
| 插件 | DeathChest | 死亡掉落箱子插件 | Java | MIT | [repo](https://github.com/OrzMC/death-chest) |
| 插件 | EzShops | 商店插件 | Java | MIT | [repo](https://github.com/OrzMC/EzShops) |
| CLI/工具 | **orzmc-app** | 跨平台 CLI：客户端启动 / 服务端一键部署，`pip install orzmc-app` | Python | Apache-2.0 | [PyPI](https://pypi.org/project/orzmc-app/) |
| CLI/工具 | **OrzMCAdmin** | 服主自动化运维，可交给 AI Agent 处理 | Python | MIT | [repo](https://github.com/OrzMC/OrzMCAdmin) |
| CLI/工具 | **OrzMCBackup** | MCA 世界备份 / 优化，按 InhabitedTime 清理区块 | Kotlin | [占位] | [repo](https://github.com/OrzMC/OrzMCBackup) |
| CLI/工具 | rust-thanos | Rust 版区块清理工具 | Rust | [占位] | [repo](https://github.com/OrzMC/rust-thanos) |
| CLI/工具 | thanos | PHP 版区块清理工具（上游 fork） | PHP | [占位] | [repo](https://github.com/aternosorg/thanos) |
| 部署/网络 | **OrzMCDeploy** | Docker 容器化部署：MCSManager / EasyBot / MariaDB / Gatus | Shell | [占位] | [repo](https://github.com/OrzMC/OrzMCDeploy) |
| 部署/网络 | **OrzMCProxy** | FRP 跨网中转代理，解决国内三网互联延迟高 / 拒连 | Shell | [占位] | [repo](https://github.com/OrzMC/OrzMCProxy) |
| 客户端/应用 | **OrzMCApp** | macOS/iOS 应用 + Swift 库 | Swift | [占位] | [repo](https://github.com/OrzMC/OrzMCApp) |
| 客户端/应用 | OrzWebMC | 浏览器玩 Minecraft 的探索 | [占位] | [占位] | [repo](https://github.com/OrzMC/OrzWebMC) |
| 站点/社区 | **OrzMCSite** | 官方网站 orzmc.jokerhub.cn | HTML | [占位] | [官网](https://orzmc.jokerhub.cn) |
| 运维脚本 | scripts/ · skins/ | 服务器运维脚本 / 玩家皮肤 | Shell | — | 见 [OrzMC](https://github.com/OrzMC/OrzMC) |

## 🎮 玩家专区

进服三步：**申请白名单 → 审核通过 → 进服**（审核制，保证社区质量）。

| 信息 | 值 |
|---|---|
| 服务器地址 | `[占位: 国内服]` / `[占位: 海外服]` |
| 游戏版本 | `[占位: 如 1.21.x]` |
| 客户端 | Java 版，推荐对应版本，可用 orzmc-app 一键启动 |

**服务器特色**
- PaperMC 核心，性能稳定
- 强制白名单 + 审核制进服
- 国内 / 海外双服**隔离地图**
- 海外服**按需启停**（省钱、省资源）
- 遵守 Mojang EULA，纯净合规
- TNT 防护 / 区域限制 / 跨服传送门

**社群入口**
🌐 官网白名单申请页 `[占位]` · QQ 群 `[占位]` · Discord `[占位]` · 𝕏 [@OrzMC666](https://x.com/OrzMC666)

## 👨‍💻 开发者专区

全栈 Minecraft 开源矩阵，从插件到网络到客户端，总有一块适合你。

| 技术栈 | 相关项目 |
|---|---|
| Java 21 · Gradle · PaperMC API | OrzMCPlugin + 工具插件 |
| Python · PyPI · CLI | orzmc-app、OrzMCAdmin |
| Kotlin · JVM | OrzMCBackup |
| Rust | rust-thanos |
| Swift · SwiftUI | OrzMCApp |
| Shell · Docker · FRP | OrzMCDeploy、OrzMCProxy、scripts/ |
| HTML · JS | OrzMCSite、OrzWebMC |

**如何贡献**
1. 从 [OrzMC](https://github.com/OrzMC/OrzMC) 找到感兴趣的仓库
2. fork → 新建分支 → 提交 → 提交 PR
3. 遵循各仓库的 CONTRIBUTING / CODE_OF_CONDUCT

**新手任务**
- 找各仓库 Issues 里的 `good first issue` 标签 `[占位: 贴具体 issue 链接]`
- 想快速上手？先 `pip install orzmc-app` 体验 CLI，再读它的源码

**如何跑起来**
- 插件：`cd plugin && ./gradlew build`
- CLI：`pip install orzmc-app` 或官网安装脚本
- 部署：参考 [OrzMCDeploy](https://github.com/OrzMC/OrzMCDeploy) 的 docker-compose

**代码规范**
- Java：遵循 PaperMC 上游惯例，Gradle + spotless / checkstyle
- Python：ruff + mypy
- Kotlin / Rust / Swift / Shell：各语言官方格式化工具
- Commit 与分支规范见各仓库 CONTRIBUTING

## 🗺️ 近期动态

- [ ] 白名单申请流程线上化
- [ ] 插件增值功能（付费档）上线
- [ ] 海外服自动启停稳定化
- [ ] 更多 good-first-issue 帮助新人加入
- [ ] 官网 2.0（OrzMCSite）

## 💖 支持我们

OrzMC 正在从「用爱发电」走向**混合自营利**：核心功能永久免费，付费用于维持运营与激励贡献者，让社区长期活下去。

**资金去向（透明公开）**

| 用途 | 说明 |
|---|---|
| 服务器 | 国内 + 海外双服机器 / 带宽 |
| 域名与 CDN | orzmc.jokerhub.cn |
| CI / 构建 | GitHub Actions、签名、发布 |
| 开发激励 | 向活跃贡献者回馈 |

**❤️ 无偿支持档（捐赠）**
- GitHub Sponsors `[占位]` · 爱发电 `[占位]`
- 回馈：资金去向每月公开；可选加入赞助者名单

**🚀 增值档（开源核心免费 + 高级功能付费）**
- 插件高级功能解锁、优先功能排期、一对一技术支持、提前体验
- 定价与说明 `[占位: 商品页 / 定价表链接]`

**🛠️ 专业服务档（代部署 / 代运维）**
- 代部署 PaperMC 私服、长期代运维、定制插件 / 脚本、服务器迁移
- 联系方式 `[占位: 官网工单链接 / 邮箱]`

---

**链接汇总**：🌐 [官网](https://orzmc.jokerhub.cn) · [Modrinth](https://modrinth.com/organization/orzmc) · [Hangar](https://hangar.papermc.io/wangzhizhou666) · 𝕏 [@OrzMC666](https://x.com/OrzMC666) · [GitHub 组织](https://github.com/OrzMC)

**许可证**：组内各仓库独立许可，以 Apache-2.0 / MIT / GPL-3.0 为主，详见各仓库 LICENSE。

**联系**：`[占位: 联系邮箱]` · 官网表单

_Made with ❤️ in China · 遵循 Mojang EULA · 与 Mojang / Microsoft 无关_
