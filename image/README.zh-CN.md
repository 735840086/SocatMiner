<div align="center">

# SocatMiner

**下一代高性能矿池代理与节点管理系统**

<p>
  <a href="https://github.com/SocatMiner/SocatMiner/releases">
    <img src="https://img.shields.io/github/v/tag/SocatMiner/SocatMiner?label=版本&color=0EA5E9&logo=semver&logoColor=white" alt="Version">
  </a>
  <a href="LICENSE">
    <img src="https://img.shields.io/badge/许可证-MIT-22C55E?logo=open-source-initiative&logoColor=white" alt="License">
  </a>
  <a href="https://github.com/SocatMiner/SocatMiner">
    <img src="https://img.shields.io/github/stars/SocatMiner/SocatMiner?style=flat&color=F59E0B&logo=github" alt="GitHub stars">
  </a>
  <img src="https://img.shields.io/badge/性能-100K%20并发-8B5CF6?logo=lightning&logoColor=white" alt="Performance">
  <img src="https://img.shields.io/badge/Rust-1.75%2B-DEA584?logo=rust&logoColor=white" alt="Rust Version">
</p>

<p>
  <a href="https://socatminer.org">官方网站</a>
  ·
  <a href="https://docs.socatminer.org">文档中心</a>
  ·
  <a href="https://github.com/SocatMiner/SocatMiner/releases">更新日志</a>
  ·
  <a href="#联系方式">商务合作</a>
</p>

<p>
  <strong>简体中文</strong>
  ·
  <a href="README.en-US.md">English</a>
</p>

<img src="https://raw.githubusercontent.com/SocatMiner/assets/main/banner.png" alt="SocatMiner 产品预览" width="900" style="border-radius: 12px; box-shadow: 0 10px 40px rgba(0,0,0,0.3);">

</div>

---

## 🚀 项目简介

**SocatMiner** 是一款基于 Rust 语言构建的企业级矿池代理与全链路节点管理系统。专为大规模矿场、矿池节点运营商和专业运维团队设计，提供高性能连接转发、智能负载均衡、多链费率管理与可视化实时监控等核心能力。

采用零拷贝异步架构，单节点可支撑 **100,000+** 矿机并发连接，延迟低于 **1ms**。配合 SocatMiner Secure Client 实现端到端加密传输，有效抵御中间人攻击与流量嗅探。

> **设计理念**：稳定优先 · 性能极致 · 运维友好 · 合规透明

---

## ✨ 核心特性

<div align="center">

| 特性 | 说明 |
|:---:|:---|
| 🎯 **矿池代理转发** | 支持 30+ 主流挖矿算法，无缝对接全球各大矿池，智能路由与故障自动切换 |
| ⚡ **自建矿池节点** | 一键部署 Stratum 节点，支持自定义费率、算力拆分与多级账户体系 |
| 🔐 **安全传输隧道** | 自研加密协议 + TLS 1.3 双重保护，配合本地客户端实现数据压缩与链路加密 |
| 📊 **实时监控大屏** | Web 管理后台提供算力趋势、在线状态、收益统计等多维度可视化仪表盘 |
| 🌐 **多平台部署** | Linux / Windows / macOS / ARM64 / ARMV7 全架构支持，Docker 一键部署 |
| 🔧 **API 与 Webhook** | 完整的 RESTful API 与事件回调，轻松对接自有运维平台与告警系统 |
| 🧩 **插件化架构** | 支持自定义认证模块、计费插件与数据导出，满足企业级定制需求 |
| 🛡️ **DDoS 防护** | 内置连接限速、IP 黑名单与异常流量识别，保障节点稳定运行 |

</div>

---

## 💰 支持币种

<div align="center">

### 主流币种

<img src="https://cdn.jsdelivr.net/gh/atomiclabs/cryptocurrency-icons@16edb8e652a0c43c58c3d7e4a7b7c6f9a0e4d3c2/svg/color/btc.svg" alt="Bitcoin" title="Bitcoin (BTC)" height="40" hspace="8">
<img src="https://cdn.jsdelivr.net/gh/atomiclabs/cryptocurrency-icons@16edb8e652a0c43c58c3d7e4a7b7c6f9a0e4d3c2/svg/color/eth.svg" alt="Ethereum" title="EthereumPoW (ETHW)" height="40" hspace="8">
<img src="https://cdn.jsdelivr.net/gh/atomiclabs/cryptocurrency-icons@16edb8e652a0c43c58c3d7e4a7b7c6f9a0e4d3c2/svg/color/etc.svg" alt="Ethereum Classic" title="Ethereum Classic (ETC)" height="40" hspace="8">
<img src="https://cdn.jsdelivr.net/gh/atomiclabs/cryptocurrency-icons@16edb8e652a0c43c58c3d7e4a7b7c6f9a0e4d3c2/svg/color/ltc.svg" alt="Litecoin" title="Litecoin (LTC)" height="40" hspace="8">
<img src="https://cdn.jsdelivr.net/gh/atomiclabs/cryptocurrency-icons@16edb8e652a0c43c58c3d7e4a7b7c6f9a0e4d3c2/svg/color/bch.svg" alt="Bitcoin Cash" title="Bitcoin Cash (BCH)" height="40" hspace="8">
<img src="https://cdn.jsdelivr.net/gh/atomiclabs/cryptocurrency-icons@16edb8e652a0c43c58c3d7e4a7b7c6f9a0e4d3c2/svg/color/zec.svg" alt="Zcash" title="Zcash (ZEC)" height="40" hspace="8">
<img src="https://cdn.jsdelivr.net/gh/atomiclabs/cryptocurrency-icons@16edb8e652a0c43c58c3d7e4a7b7c6f9a0e4d3c2/svg/color/dash.svg" alt="Dash" title="Dash (DASH)" height="40" hspace="8">
<img src="https://cdn.jsdelivr.net/gh/atomiclabs/cryptocurrency-icons@16edb8e652a0c43c58c3d7e4a7b7c6f9a0e4d3c2/svg/color/xmr.svg" alt="Monero" title="Monero (XMR)" height="40" hspace="8">

### 热门新兴币种

<img src="https://cdn.jsdelivr.net/gh/atomiclabs/cryptocurrency-icons@16edb8e652a0c43c58c3d7e4a7b7c6f9a0e4d3c2/svg/color/kas.svg" alt="Kaspa" title="Kaspa (KAS)" height="36" hspace="6">
<img src="https://cdn.jsdelivr.net/gh/atomiclabs/cryptocurrency-icons@16edb8e652a0c43c58c3d7e4a7b7c6f9a0e4d3c2/svg/color/rvn.svg" alt="Ravencoin" title="Ravencoin (RVN)" height="36" hspace="6">
<img src="https://cdn.jsdelivr.net/gh/atomiclabs/cryptocurrency-icons@16edb8e652a0c43c58c3d7e4a7b7c6f9a0e4d3c2/svg/color/cfx.svg" alt="Conflux" title="Conflux (CFX)" height="36" hspace="6">
<img src="https://cdn.jsdelivr.net/gh/atomiclabs/cryptocurrency-icons@16edb8e652a0c43c58c3d7e4a7b7c6f9a0e4d3c2/svg/color/erg.svg" alt="Ergo" title="Ergo (ERG)" height="36" hspace="6">
<img src="https://cdn.jsdelivr.net/gh/atomiclabs/cryptocurrency-icons@16edb8e652a0c43c58c3d7e4a7b7c6f9a0e4d3c2/svg/color/zen.svg" alt="Horizen" title="Horizen (ZEN)" height="36" hspace="6">
<img src="https://cdn.jsdelivr.net/gh/atomiclabs/cryptocurrency-icons@16edb8e652a0c43c58c3d7e4a7b7c6f9a0e4d3c2/svg/color/aleph.svg" alt="Alephium" title="Alephium (ALPH)" height="36" hspace="6">
<img src="https://cdn.jsdelivr.net/gh/atomiclabs/cryptocurrency-icons@16edb8e652a0c43c58c3d7e4a7b7c6f9a0e4d3c2/svg/color/nexa.svg" alt="Nexa" title="Nexa (NEXA)" height="36" hspace="6">
<img src="https://cdn.jsdelivr.net/gh/atomiclabs/cryptocurrency-icons@16edb8e652a0c43c58c3d7e4a7b7c6f9a0e4d3c2/svg/color/ckb.svg" alt="Nervos" title="Nervos (CKB)" height="36" hspace="6">

</div>

<details>
<summary><strong>📋 完整算法支持列表</strong></summary>

| 算法 | 支持币种 |
|:---|:---|
| **SHA256** | BTC、BCH、SPACE、NMC |
| **Ethash / Etchash** | ETC、ETHW、ETHF、OCTA、CLORE、NEURAI、NEOXA、ZIL、CLO、UBQ、PWR、BTN |
| **Scrypt** | LTC、BEL、DOGE |
| **kHeavyHash** | KASPA、PYI、SDR、KLS |
| **Blake2s** | KDA |
| **Blake2b** | SC、HNS、Siacoin |
| **Octopus** | CFX |
| **DynexSolve** | DNX |
| **Eaglesong** | CKB |
| **Equihash** | ZEC、ZEN、BTG |
| **RandomX** | XMR、ZEPH、NEVO |
| **KawPow** | RVN、MEWC、AIPG |
| **Autolykos2** | ERG |
| **NexaPow** | NEXA |
| **Blake3** | ALPH、IRON |
| **GhostRider** | RTM、RTC、MECU、MAXE |
| **Cuckatoo32** | GRIN |
| **ProgPow** | SERO、FIRO |

</details>

---

## 🏊 支持矿池

<div align="center">

<table>
  <tr>
    <td align="center" width="140">
      <img src="https://www.f2pool.com/static/images/logo.png" alt="F2Pool" height="32">
      <br><sub>F2Pool 鱼池</sub>
    </td>
    <td align="center" width="140">
      <img src="https://static.antpool.com/static/images/logo.png" alt="AntPool" height="32">
      <br><sub>AntPool 蚂蚁矿池</sub>
    </td>
    <td align="center" width="140">
      <img src="https://www.poolin.com/dist/images/logo.png" alt="Poolin" height="32">
      <br><sub>Poolin 币印</sub>
    </td>
    <td align="center" width="140">
      <img src="https://www.viabtc.com/_nuxt/img/logo.3b3e6d6.png" alt="ViaBTC" height="32">
      <br><sub>ViaBTC</sub>
    </td>
  </tr>
  <tr>
    <td align="center" width="140">
      <img src="https://bin.bnbstatic.com/image/static-pool/logo-pool.png" alt="Binance Pool" height="28">
      <br><sub>Binance Pool</sub>
    </td>
    <td align="center" width="140">
      <img src="https://slushpool.com/static/media/logo.6f8a4b7e.svg" alt="Braiins Pool" height="28">
      <br><sub>Braiins (Slush) Pool</sub>
    </td>
    <td align="center" width="140">
      <img src="https://luxor.tech/wp-content/uploads/2022/03/luxor-logo-dark.svg" alt="Luxor" height="28">
      <br><sub>Luxor Tech</sub>
    </td>
    <td align="center" width="140">
      <img src="https://www.bitcoin.com/images/bitcoin-com-logo.svg" alt="Bitcoin.com" height="28">
      <br><sub>Bitcoin.com Pool</sub>
    </td>
  </tr>
  <tr>
    <td align="center" width="140">
      <img src="https://www.nicehash.com/images/nh-logo-dark.svg" alt="NiceHash" height="28">
      <br><sub>NiceHash</sub>
    </td>
    <td align="center" width="140">
      <img src="https://mining-dutch.nl/images/logo.png" alt="MiningDutch" height="28">
      <br><sub>MiningDutch</sub>
    </td>
    <td align="center" width="140">
      <img src="https://www.prohashing.com/images/logo.svg" alt="ProHashing" height="28">
      <br><sub>ProHashing</sub>
    </td>
    <td align="center" width="140">
      <img src="https://zergpool.com/img/logo.png" alt="ZergPool" height="28">
      <br><sub>ZergPool</sub>
    </td>
  </tr>
</table>

<sub>兼容所有标准 Stratum V1 / V2 协议矿池，列表持续更新中</sub>

</div>

---

## 🚀 快速部署

### 系统要求

| 配置 | 最低要求 | 推荐配置 |
|:---|:---|:---|
| **操作系统** | Ubuntu 20.04 / CentOS 8 | Ubuntu 22.04 LTS |
| **CPU** | 1 核 | 4 核及以上 |
| **内存** | 512 MB | 4 GB 及以上 |
| **带宽** | 1 Mbps | 100 Mbps 及以上 |
| **磁盘** | 10 GB SSD | 50 GB SSD |

### Linux 一键安装

> **默认管理员账号**：`admin`  **默认密码**：`socatminer2024`
>
> 首次登录后请立即修改密码并调整 Web 访问端口。

```bash
# 官方安装脚本（推荐）
bash <(curl -fsSL https://install.socatminer.org)

# GitHub 镜像源
bash <(curl -fsSL https://raw.githubusercontent.com/SocatMiner/SocatMiner/main/install.sh)

# ARM64 架构
bash <(curl -fsSL https://install.socatminer.org/arm64.sh)

# ARMV7 架构
bash <(curl -fsSL https://install.socatminer.org/armv7.sh)
```

安装完成后，访问 `http://服务器IP:端口号` 进入管理后台。

### Docker 部署

```bash
# 拉取镜像
docker pull socatminer/socatminer:latest

# 启动容器
docker run -d \
  --name socatminer \
  --restart unless-stopped \
  -p 8080:8080 \
  -p 3333-3350:3333-3350 \
  -v /opt/socatminer:/data \
  socatminer/socatminer:latest
```

### Windows 部署

1. 前往 [Releases 页面](https://github.com/SocatMiner/SocatMiner/releases) 下载最新 Windows 版本
2. 解压至任意目录，以管理员身份运行 `SocatMiner.exe`
3. 根据终端提示访问 Web 管理界面

---

## 🏗️ 系统架构

```
                        ┌─────────────────────────┐
                        │   SocatMiner 管理面板    │
                        │   (Web Dashboard)       │
                        └───────────┬─────────────┘
                                    │
                        ┌───────────▼─────────────┐
                        │   核心控制引擎 (Core)    │
                        │  ┌───────────────────┐  │
                        │  │  配置管理中心      │  │
                        │  │  认证与权限        │  │
                        │  │  数据持久化        │  │
                        │  └───────────────────┘  │
                        └───────────┬─────────────┘
                                    │
        ┌───────────────────────────┼───────────────────────────┐
        │                           │                           │
┌───────▼───────┐         ┌─────────▼─────────┐       ┌─────────▼─────────┐
│  Stratum 节点  │         │   矿池代理网关     │       │  安全隧道服务      │
│  (自建矿池)    │         │  (Pool Proxy)     │       │  (Secure Tunnel)  │
│               │         │                   │       │                   │
│ • 份额验证    │         │ • 协议转换        │       │ • TLS 1.3 加密    │
│ • 难度调整    │         │ • 负载均衡        │       │ • 数据压缩        │
│ • 收益计算    │         │ • 故障转移        │       │ • 链路复用        │
│ • 支付模块    │         │ • 算力统计        │       │ • 防嗅探          │
└───────────────┘         └─────────┬─────────┘       └─────────┬─────────┘
                                    │                           │
                            ┌───────▼───────┐           ┌───────▼───────┐
                            │  目标矿池集群  │           │  矿机本地客户端  │
                            │ (全球多节点)   │           │ (SMC Client)   │
                            └───────────────┘           └───────────────┘
```

---

## 📊 性能基准

| 指标 | 数值 | 说明 |
|:---|:---:|:---|
| **最大并发连接** | 100,000+ | 单节点 4 核 8G 环境 |
| **转发延迟** | < 1 ms | 内网环境 P99 延迟 |
| **内存占用** | ~ 2 MB / 千连接 | 极低内存开销 |
| **CPU 使用率** | < 5% @ 1万连接 | 异步非阻塞架构 |
| **崩溃恢复时间** | < 3 秒 | 进程守护自动重启 |
| **日算力统计精度** | 99.9% | 份额级精确统计 |

---

## 📚 文档导航

| 文档 | 链接 | 适用人群 |
|:---|:---|:---|
| 🚀 **快速入门指南** | [点击查看](https://docs.socatminer.org/quickstart) | 新手用户 |
| ⚙️ **矿池代理配置** | [点击查看](https://docs.socatminer.org/pool-proxy) | 矿场运维 |
| 🏗️ **自建节点部署** | [点击查看](https://docs.socatminer.org/node-setup) | 节点运营商 |
| 🔐 **安全客户端使用** | [点击查看](https://docs.socatminer.org/secure-client) | 所有用户 |
| 📡 **API 接口文档** | [点击查看](https://docs.socatminer.org/api) | 开发者 |
| ❓ **常见问题 FAQ** | [点击查看](https://docs.socatminer.org/faq) | 所有用户 |

---

## 🌐 社区与支持

<div align="center">

[![Telegram](https://img.shields.io/badge/Telegram-官方群组-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/socatminer)
[![Discord](https://img.shields.io/badge/Discord-加入社区-5865F2?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/socatminer)
[![Twitter/X](https://img.shields.io/badge/X-@socatminer-000000?style=for-the-badge&logo=x&logoColor=white)](https://x.com/socatminer)
[![GitHub Issues](https://img.shields.io/badge/GitHub-提交问题-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/SocatMiner/SocatMiner/issues)

</div>

### 商务合作

如需企业定制、OEM 授权、技术支持或节点合作，请通过以下方式联系我们：

- 📧 商务邮箱：`business@socatminer.org`
- 💬 Telegram：`@socatminer_admin`
- 📋 合作咨询：[提交表单](https://socatminer.org/contact)

---

## ⚖️ 法律声明

> [!WARNING]
> **合规使用提示**
>
> SocatMiner 受香港特别行政区法律管辖。不同国家和地区对数字货币挖矿相关活动的监管要求存在差异。
>
> 使用本软件前，请确保您所在司法管辖区允许开展数字货币挖矿及相关服务活动。用户需自行承担因违反当地法律法规而产生的全部责任。

<details>
<summary><strong>📜 完整服务条款</strong></summary>

### 1. 软件性质
SocatMiner 是一款矿池协议转发与节点管理工具，不属于 VPN 或网络代理类产品，不具备突破网络限制或访问被禁止内容的功能。

### 2. 使用前提
- 您确认拥有所接入矿机的完整所有权或合法管理权限
- 所有接入设备均由设备所有者主动配置连接地址
- 您不在任何恐怖主义组织及制裁名单之中
- 您所在地区允许开展数字货币相关活动

### 3. 受限地区
本软件不向以下地区用户提供服务：
- 中国大陆地区
- 古巴、伊朗、朝鲜、叙利亚等受国际制裁国家
- 其他明确禁止数字货币挖矿活动的司法管辖区

### 4. 免责声明
- 本软件按"现状"提供，不提供任何明示或暗示的担保
- 因使用本软件产生的任何直接或间接损失，开发者不承担责任
- 如因当地法律法规导致使用本软件违法，全部责任由使用者自行承担

使用本软件即视为您已阅读并同意以上全部条款。

</details>

---

## 📄 许可证

本项目基于 [MIT License](LICENSE) 开源发布。

---

<div align="center">

**如果本项目对您有帮助，欢迎点亮 ⭐ Star 支持我们**

Made with ❤️ by SocatMiner Team

</div>
