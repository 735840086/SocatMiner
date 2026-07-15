<div align="center">

# SocatMiner

**Next-Gen High-Performance Mining Pool Proxy & Node Management System**

<p>
  <a href="https://github.com/SocatMiner/SocatMiner/releases">
    <img src="https://img.shields.io/github/v/tag/SocatMiner/SocatMiner?label=Version&color=0EA5E9&logo=semver&logoColor=white" alt="Version">
  </a>
  <a href="LICENSE">
    <img src="https://img.shields.io/badge/License-MIT-22C55E?logo=open-source-initiative&logoColor=white" alt="License">
  </a>
  <a href="https://github.com/SocatMiner/SocatMiner">
    <img src="https://img.shields.io/github/stars/SocatMiner/SocatMiner?style=flat&color=F59E0B&logo=github" alt="GitHub stars">
  </a>
  <img src="https://img.shields.io/badge/Performance-100K%20Connections-8B5CF6?logo=lightning&logoColor=white" alt="Performance">
  <img src="https://img.shields.io/badge/Rust-1.75%2B-DEA584?logo=rust&logoColor=white" alt="Rust Version">
</p>

<p>
  <a href="https://socatminer.org">Official Website</a>
  ·
  <a href="https://docs.socatminer.org">Documentation</a>
  ·
  <a href="https://github.com/SocatMiner/SocatMiner/releases">Changelog</a>
  ·
  <a href="#contact">Business Contact</a>
</p>

<p>
  <a href="README.zh-CN.md">简体中文</a>
  ·
  <strong>English</strong>
</p>

<img src="https://raw.githubusercontent.com/SocatMiner/assets/main/banner.png" alt="SocatMiner Product Preview" width="900" style="border-radius: 12px; box-shadow: 0 10px 40px rgba(0,0,0,0.3);">

</div>

---

## 🚀 Introduction

**SocatMiner** is an enterprise-grade mining pool proxy and full-stack node management system built in Rust. Designed for large-scale mining farms, pool node operators, and professional DevOps teams, it provides high-performance connection forwarding, intelligent load balancing, multi-chain fee management, and real-time visual monitoring.

Powered by a zero-copy async architecture, a single node can handle **100,000+** concurrent miner connections with sub-**1ms** latency. Combined with the SocatMiner Secure Client, it enables end-to-end encrypted transmission, effectively mitigating MITM attacks and traffic sniffing.

> **Design Philosophy**: Stability First · Extreme Performance · Ops-Friendly · Compliance & Transparency

---

## ✨ Core Features

<div align="center">

| Feature | Description |
|:---:|:---|
| 🎯 **Pool Proxy Forwarding** | Supports 30+ major mining algorithms, seamless integration with global mining pools, smart routing and automatic failover |
| ⚡ **Self-Hosted Pool Node** | One-click Stratum node deployment with custom fees, hashrate splitting, and multi-level account system |
| 🔐 **Secure Transport Tunnel** | Proprietary encryption protocol + TLS 1.3 dual protection with data compression and link encryption via local client |
| 📊 **Real-Time Monitoring** | Web dashboard with multi-dimensional visualizations: hashrate trends, online status, earnings statistics, and more |
| 🌐 **Multi-Platform Deployment** | Full architecture support: Linux / Windows / macOS / ARM64 / ARMV7, one-click Docker deployment |
| 🔧 **API & Webhooks** | Complete RESTful API and event callbacks for easy integration with your own operations and alerting systems |
| 🧩 **Plugin Architecture** | Custom auth modules, billing plugins, and data exports to meet enterprise customization needs |
| 🛡️ **DDoS Protection** | Built-in rate limiting, IP blacklisting, and anomaly detection to ensure node stability |

</div>

---

## 💰 Supported Coins

<div align="center">

### Major Cryptocurrencies

<img src="https://cdn.jsdelivr.net/gh/atomiclabs/cryptocurrency-icons@16edb8e652a0c43c58c3d7e4a7b7c6f9a0e4d3c2/svg/color/btc.svg" alt="Bitcoin" title="Bitcoin (BTC)" height="40" hspace="8">
<img src="https://cdn.jsdelivr.net/gh/atomiclabs/cryptocurrency-icons@16edb8e652a0c43c58c3d7e4a7b7c6f9a0e4d3c2/svg/color/eth.svg" alt="Ethereum" title="EthereumPoW (ETHW)" height="40" hspace="8">
<img src="https://cdn.jsdelivr.net/gh/atomiclabs/cryptocurrency-icons@16edb8e652a0c43c58c3d7e4a7b7c6f9a0e4d3c2/svg/color/etc.svg" alt="Ethereum Classic" title="Ethereum Classic (ETC)" height="40" hspace="8">
<img src="https://cdn.jsdelivr.net/gh/atomiclabs/cryptocurrency-icons@16edb8e652a0c43c58c3d7e4a7b7c6f9a0e4d3c2/svg/color/ltc.svg" alt="Litecoin" title="Litecoin (LTC)" height="40" hspace="8">
<img src="https://cdn.jsdelivr.net/gh/atomiclabs/cryptocurrency-icons@16edb8e652a0c43c58c3d7e4a7b7c6f9a0e4d3c2/svg/color/bch.svg" alt="Bitcoin Cash" title="Bitcoin Cash (BCH)" height="40" hspace="8">
<img src="https://cdn.jsdelivr.net/gh/atomiclabs/cryptocurrency-icons@16edb8e652a0c43c58c3d7e4a7b7c6f9a0e4d3c2/svg/color/zec.svg" alt="Zcash" title="Zcash (ZEC)" height="40" hspace="8">
<img src="https://cdn.jsdelivr.net/gh/atomiclabs/cryptocurrency-icons@16edb8e652a0c43c58c3d7e4a7b7c6f9a0e4d3c2/svg/color/dash.svg" alt="Dash" title="Dash (DASH)" height="40" hspace="8">
<img src="https://cdn.jsdelivr.net/gh/atomiclabs/cryptocurrency-icons@16edb8e652a0c43c58c3d7e4a7b7c6f9a0e4d3c2/svg/color/xmr.svg" alt="Monero" title="Monero (XMR)" height="40" hspace="8">

### Popular Emerging Coins

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
<summary><strong>📋 Full Algorithm Support List</strong></summary>

| Algorithm | Supported Coins |
|:---|:---|
| **SHA256** | BTC, BCH, SPACE, NMC |
| **Ethash / Etchash** | ETC, ETHW, ETHF, OCTA, CLORE, NEURAI, NEOXA, ZIL, CLO, UBQ, PWR, BTN |
| **Scrypt** | LTC, BEL, DOGE |
| **kHeavyHash** | KASPA, PYI, SDR, KLS |
| **Blake2s** | KDA |
| **Blake2b** | SC, HNS, Siacoin |
| **Octopus** | CFX |
| **DynexSolve** | DNX |
| **Eaglesong** | CKB |
| **Equihash** | ZEC, ZEN, BTG |
| **RandomX** | XMR, ZEPH, NEVO |
| **KawPow** | RVN, MEWC, AIPG |
| **Autolykos2** | ERG |
| **NexaPow** | NEXA |
| **Blake3** | ALPH, IRON |
| **GhostRider** | RTM, RTC, MECU, MAXE |
| **Cuckatoo32** | GRIN |
| **ProgPow** | SERO, FIRO |

</details>

---

## 🏊 Supported Mining Pools

<div align="center">

<table>
  <tr>
    <td align="center" width="140">
      <img src="https://www.f2pool.com/static/images/logo.png" alt="F2Pool" height="32">
      <br><sub>F2Pool</sub>
    </td>
    <td align="center" width="140">
      <img src="https://static.antpool.com/static/images/logo.png" alt="AntPool" height="32">
      <br><sub>AntPool</sub>
    </td>
    <td align="center" width="140">
      <img src="https://www.poolin.com/dist/images/logo.png" alt="Poolin" height="32">
      <br><sub>Poolin</sub>
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

<sub>Compatible with all standard Stratum V1 / V2 protocol pools. List continuously updated.</sub>

</div>

---

## 🚀 Quick Deployment

### System Requirements

| Component | Minimum | Recommended |
|:---|:---|:---|
| **OS** | Ubuntu 20.04 / CentOS 8 | Ubuntu 22.04 LTS |
| **CPU** | 1 Core | 4+ Cores |
| **RAM** | 512 MB | 4+ GB |
| **Bandwidth** | 1 Mbps | 100+ Mbps |
| **Storage** | 10 GB SSD | 50 GB SSD |

### Linux One-Click Install

> **Default Admin Credentials**: Username: `admin`  Password: `socatminer2024`
>
> Please change the password and adjust the Web access port immediately after first login.

```bash
# Official installer (recommended)
bash <(curl -fsSL https://install.socatminer.org)

# GitHub mirror
bash <(curl -fsSL https://raw.githubusercontent.com/SocatMiner/SocatMiner/main/install.sh)

# ARM64 architecture
bash <(curl -fsSL https://install.socatminer.org/arm64.sh)

# ARMV7 architecture
bash <(curl -fsSL https://install.socatminer.org/armv7.sh)
```

After installation, visit `http://SERVER_IP:PORT` to access the admin dashboard.

### Docker Deployment

```bash
# Pull image
docker pull socatminer/socatminer:latest

# Start container
docker run -d \
  --name socatminer \
  --restart unless-stopped \
  -p 8080:8080 \
  -p 3333-3350:3333-3350 \
  -v /opt/socatminer:/data \
  socatminer/socatminer:latest
```

### Windows Deployment

1. Go to the [Releases page](https://github.com/SocatMiner/SocatMiner/releases) and download the latest Windows version
2. Extract to any directory, run `SocatMiner.exe` as Administrator
3. Access the Web dashboard following the terminal prompts

---

## 🏗️ System Architecture

```
                        ┌─────────────────────────┐
                        │   SocatMiner Dashboard  │
                        │      (Web UI)           │
                        └───────────┬─────────────┘
                                    │
                        ┌───────────▼─────────────┐
                        │    Core Control Engine   │
                        │  ┌───────────────────┐  │
                        │  │  Config Manager    │  │
                        │  │  Auth & Perms      │  │
                        │  │  Data Persistence  │  │
                        │  └───────────────────┘  │
                        └───────────┬─────────────┘
                                    │
        ┌───────────────────────────┼───────────────────────────┐
        │                           │                           │
┌───────▼───────┐         ┌─────────▼─────────┐       ┌─────────▼─────────┐
│ Stratum Node  │         │   Pool Proxy GW    │       │  Secure Tunnel    │
│ (Self-Hosted) │         │                   │       │    Service        │
│               │         │ • Protocol Conv.   │       │ • TLS 1.3 Encrypt │
│ • Share Verify│         │ • Load Balancing   │       │ • Data Compression│
│ • Difficulty  │         │ • Failover         │       │ • Link Multiplex  │
│ • Reward Calc │         │ • Hashrate Stats   │       │ • Anti-Sniffing   │
│ • Payout Mod  │         │                   │       │                   │
└───────────────┘         └─────────┬─────────┘       └─────────┬─────────┘
                                    │                           │
                            ┌───────▼───────┐           ┌───────▼───────┐
                            │ Target Pools  │           │  Miner Client  │
                            │ (Global)      │           │  (SMC Client)  │
                            └───────────────┘           └───────────────┘
```

---

## 📊 Performance Benchmarks

| Metric | Value | Notes |
|:---|:---:|:---|
| **Max Concurrent Connections** | 100,000+ | Single node, 4 cores / 8GB RAM |
| **Forwarding Latency** | < 1 ms | P99 latency on intranet |
| **Memory Footprint** | ~ 2 MB / 1k conns | Extremely low overhead |
| **CPU Usage** | < 5% @ 10k conns | Async non-blocking architecture |
| **Crash Recovery Time** | < 3 sec | Process watchdog auto-restart |
| **Daily Hashrate Accuracy** | 99.9% | Share-level precise statistics |

---

## 📚 Documentation

| Document | Link | Audience |
|:---|:---|:---|
| 🚀 **Quick Start Guide** | [View](https://docs.socatminer.org/quickstart) | New Users |
| ⚙️ **Pool Proxy Setup** | [View](https://docs.socatminer.org/pool-proxy) | Farm Operators |
| 🏗️ **Self-Hosted Node Guide** | [View](https://docs.socatminer.org/node-setup) | Node Operators |
| 🔐 **Secure Client Guide** | [View](https://docs.socatminer.org/secure-client) | All Users |
| 📡 **API Reference** | [View](https://docs.socatminer.org/api) | Developers |
| ❓ **FAQ** | [View](https://docs.socatminer.org/faq) | All Users |

---

## 🌐 Community & Support

<div align="center">

[![Telegram](https://img.shields.io/badge/Telegram-Official_Group-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/socatminer)
[![Discord](https://img.shields.io/badge/Discord-Join_Community-5865F2?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/socatminer)
[![Twitter/X](https://img.shields.io/badge/X-@socatminer-000000?style=for-the-badge&logo=x&logoColor=white)](https://x.com/socatminer)
[![GitHub Issues](https://img.shields.io/badge/GitHub-Report_Issue-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/SocatMiner/SocatMiner/issues)

</div>

### Business Contact

For enterprise customization, OEM licensing, technical support, or node partnerships, reach out to us:

- 📧 Business Email: `business@socatminer.org`
- 💬 Telegram: `@socatminer_admin`
- 📋 Contact Form: [Submit Inquiry](https://socatminer.org/contact)

---

## ⚖️ Legal Notice

> [!WARNING]
> **Compliance Notice**
>
> SocatMiner is governed by the laws of the Hong Kong Special Administrative Region. Regulatory requirements for cryptocurrency mining activities vary across countries and regions.
>
> Before using this software, please ensure that cryptocurrency mining and related services are permitted in your jurisdiction. Users assume full responsibility for any violations of local laws and regulations.

<details>
<summary><strong>📜 Full Terms of Service</strong></summary>

### 1. Software Nature
SocatMiner is a mining pool protocol forwarding and node management tool. It is not a VPN or proxy product and does not have the capability to bypass network restrictions or access prohibited content.

### 2. Prerequisites for Use
- You confirm full ownership or legal management authority over all connected mining devices
- All connected devices are configured with connection addresses voluntarily by their owners
- You are not listed on any terrorism organization or sanctions list
- Cryptocurrency activities are legal in your jurisdiction

### 3. Restricted Regions
This software is not available to users in:
- Mainland China
- Sanctioned countries: Cuba, Iran, North Korea, Syria, etc.
- Any other jurisdiction that explicitly prohibits cryptocurrency mining

### 4. Disclaimer
- This software is provided "as is" without any express or implied warranties
- Developers shall not be liable for any direct or indirect damages arising from use
- Users bear full responsibility for any legal violations caused by local regulations

By using this software, you acknowledge that you have read and agree to all the above terms.

</details>

---

## 📄 License

This project is released under the [MIT License](LICENSE).

---

<div align="center">

**If this project helps you, please ⭐ Star to show your support**

Made with ❤️ by SocatMiner Team

</div>
