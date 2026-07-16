<div align="center">
# SocatMiner
**高性能的矿池代理与全链路节点管理系统**
<h4 align="center">MinerProxy MinerProxy MinerProxy</h4>
<p>
  <a href="https://github.com/SocatMiner/SocatMiner/releases">
    <img src="https://img.shields.io/github/v/tag/SocatMiner/SocatMiner?label=Version&color=0EA5E9&logo=semver&logoColor=white" alt="Version">
  </a>
  <a href="LICENSE">
    <img src="https://img.shields.io/badge/许可证-MIT-22C55E?logo=open-source-initiative&logoColor=white" alt="License">
  </a>
  <a href="https://github.com/735840086/SocatMiner">
    <img src="https://img.shields.io/github/stars/SocatMiner/SocatMiner?style=flat&color=F59E0B&logo=github" alt="Stars">
  </a>
  <img src="https://img.shields.io/badge/性能-10K%20并发-8B5CF6?logo=lightning&logoColor=white" alt="Performance">
  <img src="https://img.shields.io/badge/GO-1.75%2B-DEA584?logo=GO&logoColor=white" alt="GO Version">
</p>
<p>
  <a href="https://github.com/735840086/SocatMiner">仓库地址</a>
  ·
  <a href="https://github.com/735840086/SocatMiner">文档中心</a>
  ·
  <a href="https://t.me/SocatMiner">Telegram</a>
</p>
<p>
  <strong>简体中文</strong>
  ·
  <a href="README.en-US.md">English</a>
</p>
<!-- Banner图CDN修复，替换为jsDelivr持久链接 -->
<img src="https://cdn.jsdelivr.net/gh/SocatMiner/assets@main/banner.png" alt="SocatMiner 产品预览" width="900" style="border-radius: 12px; box-shadow: 0 10px 40px rgba(0,0,0,0.3);">
</div>
---
## 🚀 简介
**SocatMiner** 是一款高性能矿机集群流量转发代理系统，矿池代理与全链路节点管理。专为大规模矿场、矿池节点转发运营商和专业运维团队设计，提供高性能连接转发、多费率管理与可视化实时监控等核心能力。
采用零拷贝异步架构，单节点可支撑 **10,000+** 矿机并发连接，延迟低。配合 Socat Proxy 实现端到端加密传输，有效抵御攻击，运营商DPI与流量嗅探。
> **设计理念**：稳定优先 · 性能极致 · 运维友好 · 极简操作
---
## ✨ 核心特性
<div align="center">
| 特性 | 说明 |
|:---:|:---|
| 🎯 **矿池代理转发** | 支持多种主流挖矿算法，稳定对接全球各大矿池 |
| ⚡ **矿池节点转发** | 一键部署 Stratum 节点，支持自定义费率、算力拆分与多级账户体系 |
| 🔐 **安全传输隧道** | 私有加密协议多重保护，配合本地安全客户端实现数据压缩与链路加密 |
| 📊 **实时监控仪表** | Web 管理后台提供算力趋势、在线状态、收益统计等多维度可视化仪表盘 |
| 🌐 **平台部署** | Linux  x86架构支持，一键部署 |
</div>
---
## 💰 支持币种
<div align="center">
### 主流币种
<!-- 全部替换稳定CDN加密货币彩色SVG图标 -->
<img src="https://cdn.jsdelivr.net/npm/@creativebrandon/cryptocurrency-icons@0.0.4/svg/color/btc.svg" alt="Bitcoin" title="Bitcoin (BTC)" height="40" hspace="8">
<img src="https://cdn.jsdelivr.net/npm/@creativebrandon/cryptocurrency-icons@0.0.4/svg/color/eth.svg" alt="EthereumPoW" title="EthereumPoW (ETHW)" height="40" hspace="8">
<img src="https://cdn.jsdelivr.net/npm/@creativebrandon/cryptocurrency-icons@0.0.4/svg/color/etc.svg" alt="Ethereum Classic" title="Ethereum Classic (ETC)" height="40" hspace="8">
<img src="https://cdn.jsdelivr.net/npm/@creativebrandon/cryptocurrency-icons@0.0.4/svg/color/ltc.svg" alt="Litecoin" title="Litecoin (LTC)" height="40" hspace="8">
<img src="https://cdn.jsdelivr.net/npm/@creativebrandon/cryptocurrency-icons@0.0.4/svg/color/bch.svg" alt="Bitcoin Cash" title="Bitcoin Cash (BCH)" height="40" hspace="8">
<img src="https://cdn.jsdelivr.net/npm/@creativebrandon/cryptocurrency-icons@0.0.4/svg/color/zec.svg" alt="Zcash" title="Zcash (ZEC)" height="40" hspace="8">
<img src="https://cdn.jsdelivr.net/npm/@creativebrandon/cryptocurrency-icons@0.0.4/svg/color/dash.svg" alt="Dash" title="Dash (DASH)" height="40" hspace="8">
<img src="https://cdn.jsdelivr.net/npm/@creativebrandon/cryptocurrency-icons@0.0.4/svg/color/xmr.svg" alt="Monero" title="Monero (XMR)" height="40" hspace="8">
### 热门新兴币种
<img src="https://cdn.jsdelivr.net/npm/@creativebrandon/cryptocurrency-icons@0.0.4/svg/color/kas.svg" alt="Kaspa" title="Kaspa (KAS)" height="36" hspace="6">
<img src="https://cdn.jsdelivr.net/npm/@creativebrandon/cryptocurrency-icons@0.0.4/svg/color/rvn.svg" alt="Ravencoin" title="Ravencoin (RVN)" height="36" hspace="6">
<img src="https://cdn.jsdelivr.net/npm/@creativebrandon/cryptocurrency-icons@0.0.4/svg/color/cfx.svg" alt="Conflux" title="Conflux (CFX)" height="36" hspace="6">
<img src="https://cdn.jsdelivr.net/npm/@creativebrandon/cryptocurrency-icons@0.0.4/svg/color/erg.svg" alt="Ergo" title="Ergo (ERG)" height="36" hspace="6">
<img src="https://cdn.jsdelivr.net/npm/@creativebrandon/cryptocurrency-icons@0.0.4/svg/color/zen.svg" alt="Horizen" title="Horizen (ZEN)" height="36" hspace="6">
<img src="https://cdn.jsdelivr.net/npm/@creativebrandon/cryptocurrency-icons@0.0.4/svg/color/aleph.svg" alt="Alephium" title="Alephium (ALPH)" height="36" hspace="6">
<img src="https://cdn.jsdelivr.net/npm/@creativebrandon/cryptocurrency-icons@0.0.4/svg/color/nexa.svg" alt="Nexa" title="Nexa (NEXA)" height="36" hspace="6">
<img src="https://cdn.jsdelivr.net/npm/@creativebrandon/cryptocurrency-icons@0.0.4/svg/color/ckb.svg" alt="Nervos" title="Nervos (CKB)" height="36" hspace="6">
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
      <img src="https://cdn.jsdelivr.net/gh/SocatMiner/assets@minerpools/f2pool.png" alt="F2Pool" height="32">
      <br><sub>F2Pool 鱼池</sub>
    </td>
    <td align="center" width="140">
      <img src="https://cdn.jsdelivr.net/gh/SocatMiner/assets@minerpools/antpool.png" alt="AntPool" height="32">
      <br><sub>AntPool 蚂蚁矿池</sub>
    </td>
    <td align="center" width="140">
      <img src="https://cdn.jsdelivr.net/gh/SocatMiner/assets@minerpools/poolin.png" alt="Poolin" height="32">
      <br><sub>Poolin 币印</sub>
    </td>
    <td align="center" width="140">
      <img src="https://cdn.jsdelivr.net/gh/SocatMiner/assets@minerpools/viabtc.png" alt="ViaBTC" height="32">
      <br><sub>ViaBTC</sub>
    </td>
  </tr>
  <tr>
    <td align="center" width="140">
      <img src="https://cdn.jsdelivr.net/gh/SocatMiner/assets@minerpools/binance.png" alt="Binance Pool" height="28">
      <br><sub>Binance Pool</sub>
    </td>
    <td align="center" width="140">
      <img src="https://cdn.jsdelivr.net/gh/SocatMiner/assets@minerpools/slushpool.svg" alt="Braiins Pool" height="28">
      <br><sub>Braiins (Slush) Pool</sub>
    </td>
    <td align="center" width="140">
      <img src="https://cdn.jsdelivr.net/gh/SocatMiner/assets@minerpools/luxor.svg" alt="Luxor" height="28">
      <br><sub>Luxor Tech</sub>
    </td>
    <td align="center" width="140">
      <img src="https://cdn.jsdelivr.net/gh/SocatMiner/assets@minerpools/bitcoincom.svg" alt="Bitcoin.com" height="28">
      <br><sub>Bitcoin.com Pool</sub>
    </td>
  </tr>
  <tr>
    <td align="center" width="140">
      <img src="https://cdn.jsdelivr.net/gh/SocatMiner/assets@minerpools/nicehash.svg" alt="NiceHash" height="28">
      <br><sub>NiceHash</sub>
    </td>
    <td align="center" width="140">
      <img src="https://cdn.jsdelivr.net/gh/SocatMiner/assets@minerpools/miningdutch.png" alt="MiningDutch" height="28">
      <br><sub>MiningDutch</sub>
    </td>
    <td align="center" width="140">
      <img src="https://cdn.jsdelivr.net/gh/SocatMiner/assets@minerpools/prohashing.svg" alt="ProHashing" height="28">
      <br><sub>ProHashing</sub>
    </td>
    <td align="center" width="140">
      <img src="https://cdn.jsdelivr.net/gh/SocatMiner/assets@minerpools/zergpool.png" alt="ZergPool" height="28">
      <br><sub>ZergPool</sub>
    </td>
  </tr>
</table>
<sub>兼容所有标准 Stratum 协议矿池</sub>
</div>
---
## 🚀 快速部署
### 系统要求
| 配置 | 最低要求 | 推荐配置 |
|:---|:---|:---|
| **操作系统** | Ubuntu 20.04 / CentOS 8 | Ubuntu 22.04 LTS |
| **CPU** | 0.5 核 | 2 核及以上 |
| **内存** | 512 MB | 2 GB 及以上 |
| **带宽** | 10 Mbps | 100 Mbps 及以上 |
| **磁盘** | 20 GB SSD | 50 GB SSD |
### Linux 一键安装
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/735840086/hhminer/main/hhminer.sh)"

### Linux 一键安装

>
```安装脚本（推荐）

/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/735840086/hhminer/main/hhminer.sh)"

```

安装完成后，访问 `https://服务器IP:端口号` 进入web管理后台。


## 📊 性能基准

| 指标 | 数值 | 说明 |
|:---|:---:|:---|
| **最大并发连接** | 10,000+ | 单节点 4 核 8G 环境 |
| **转发延迟** | < 1 ms | 内网环境 P99 延迟 |
| **内存占用** | ~ 100 MB / 千连接 | 极低内存开销 |
| **CPU 使用率** | < 5% @ / 千连接 | 异步非阻塞架构 |
| **崩溃恢复时间** | < 3 秒 | 进程守护自动重启 |
| **日算力统计精度** | 99.9% | 份额级精确统计 |

---

## 📚 安全客户端

| 🔐 **安全传输隧道** | 私有加密协议多重保护，配合本地安全客户端实现数据压缩与链路加密 |

| 🔐 **安全客户端使用** | [点击查看](https://github.com/735840086/SocatProxy) 

---

## 🌐 社区与支持

<div align="center">

[![Telegram](https://img.shields.io/badge/Telegram-Telegram群组-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/SocatMiner)
[![Discord](https://img.shields.io/badge/Discord-加入社区-5865F2?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/socatminer)
[![Twitter/X](https://img.shields.io/badge/X-@socatminer-000000?style=for-the-badge&logo=x&logoColor=white)](https://x.com/socatminer)
[![GitHub Issues](https://img.shields.io/badge/GitHub-提交问题-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/SocatMiner/SocatMiner/issues)

</div>

### 😊 **特别感谢**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<img src="/image/1.png" alt="Logo" width="150">

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<img src="/image/2.png" alt="Logo" width="150">

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<img src="/image/3.png" alt="Logo" width="150">


&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<img src="/image/4.png" alt="Logo" width="150">

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<img src="/image/5.png" alt="Logo" width="150">

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<img src="/image/6.png" alt="Logo" width="150">

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<img src="/image/7.png" alt="Logo" width="150">

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<img src="/image/8.png" alt="Logo" width="150">

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<img src="/image/9.png" alt="Logo" width="150">

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<img src="/image/10.png" alt="Logo" width="150">

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<img src="/image/11.png" alt="Logo" width="150">

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<img src="/image/12.png" alt="Logo" width="150">

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<img src="/image/13.png" alt="Logo" width="150">

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<img src="/image/14.png" alt="Logo" width="150">

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<img src="/image/15.png" alt="Logo" width="150">

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<img src="/image/16.png" alt="Logo" width="150">

<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;😊特别感谢以上矿池提供了部分的技术支持</p>

### 合作

如需定制、技术支持或合作，请通过以下方式联系我们：

- 📧 咨询邮箱：`18628808761h@sina.cn`
- 💬 Telegram：`@cm1388s`

---

## ⚖️ 协议声明

> [!WARNING]
> **合规使用提示**
>
> SocatMiner 法律管辖，不同国家和地区对数字货币挖矿相关活动的监管要求存在差异。
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
