<div align="center">

# SocatMiner
### Next-Generation Encrypted Distributed Hashrate Gateway & Private Mining Pool Platform

<a href="#zh-doc">简体中文文档</a> ｜ <a href="#en-doc">English Documentation</a>

<br>

## Supported Cryptocurrencies
<img src="https://via.placeholder.com/48/FF9500/000?text=BTC" width="46" alt="Bitcoin">
<img src="https://via.placeholder.com/48/627EEA/fff?text=ETH" width="46" alt="Ethereum">
<img src="https://via.placeholder.com/48/39CD89/fff?text=ETC" width="46" alt="Ethereum Classic">
<img src="https://via.placeholder.com/48/00A5FF/fff?text=KAS" width="46" alt="Kaspa">
<img src="https://via.placeholder.com/48/BFBFBF/000?text=LTC" width="46" alt="Litecoin">
<img src="https://via.placeholder.com/48/924DFF/fff?text=RVN" width="46" alt="Ravencoin">
<img src="https://via.placeholder.com/48/C2A633/000?text=DOGE" width="46" alt="Dogecoin">
<img src="https://via.placeholder.com/48/171717/fff?text=CFX" width="46" alt="Conflux">
<img src="https://via.placeholder.com/48/20C997/fff?text=ZEC" width="46" alt="Zcash">
<img src="https://via.placeholder.com/48/FF6B6B/fff?text=XMR" width="46" alt="Monero">

<br>

## Compatible Global Mining Pools
<img src="https://via.placeholder.com/64x40/041538/fff?text=F2POOL" width="64" alt="F2Pool">
<img src="https://via.placeholder.com/64x40/111111/F8B91D?text=BINANCE" width="64" alt="Binance Pool">
<img src="https://via.placeholder.com/64x40/222/00B3FF?text=ANTPOOL" width="64" alt="AntPool">
<img src="https://via.placeholder.com/64x40/000/00CC65?text=BTC.COM" width="64" alt="BTC.com">
<img src="https://via.placeholder.com/64x40/333/FF6600?text=HIVEON" width="64" alt="Hiveon">
<img src="https://via.placeholder.com/64x40/111/9933FF?text=EZIL" width="64" alt="Ezil">
<img src="https://via.placeholder.com/64x40/000/FF3333?text=NICEHASH" width="64" alt="NiceHash">

<br>

> ### 🔒 Independent Original Architecture | Not a Fork / Modification of Any Open-Source Relay Project
> SocatMiner reconstructs the entire network transport layer, concurrency scheduler and encryption logic from scratch, with self-designed multi-level node cluster & commercial revenue calculation system, built for large-scale industrial mining cluster operation.

</div>

---

<a id="zh-doc"></a>
# 简体中文文档
## 项目介绍
SocatMiner 是面向工业级分布式算力集群打造的新一代加密矿机网关与私有化矿池一体化平台。
本项目**不属于任何现有挖矿转发程序二次修改、分支复刻**：
- 从零重构 Rust 异步IO并发调度内核，抛弃传统代理老旧网络模型
- 自主研发端到端二进制加密压缩私有隧道协议
- 全新设计多级节点级联架构、分层动态费率分润系统
- 原生内置轻量化单页面Web运维控制面板

针对性解决传统算力转发工具带宽消耗巨大、流量特征易被识别、单机承载算力规模有限、异地集群组网不稳定、收益抽水规则固化、缺少统一可视化监控等行业痛点。

### 核心适用场景
1. 多地域大型矿场集群统一运维管控
2. 4G/5G移动流量低成本算力组网方案
3. 商用算力中转、节点服务商盈利运营
4. 私有化独立矿池搭建，自主掌控算力与收益分配

## 核心差异化能力
1. **双运行模式无缝切换**
公矿池流量转发网关 + 私有独立矿池节点双模式，个人散户、中型托管矿场、规模化算力服务商均可匹配需求。
2. **自研高强度加密压缩隧道**
混合无损/有损压缩+全链路流量加密，传输数据体积压缩10~22倍，屏蔽Stratum协议特征指纹，抵御中间人抓包、链路劫持，大幅削减移动流量卡开销。
3. **超高单机并发承载性能**
底层异步运行时深度优化，单台标准服务器稳定承载5000+矿机并发在线，并发上限远超同类开源转发工具。
4. **精细化商业化费率系统**
支持固定抽水、时段动态费率、分组差异化抽水、上下级多级节点分润，后台实时可视化收益统计图表。
5. **全平台架构原生适配**
预编译二进制覆盖 X86_64 / ARM64 / ARMv7 / Windows，适配云服务器、工控机、树莓派、边缘嵌入式设备。
6. **一体化Web可视化运维后台**
实时总算力看板、在线设备列表、上下行流量监控、离线设备告警、批量矿工导入导出、全量运行日志导出一站式管理。
7. **极简一键自动化部署**
Linux 单条curl脚本全自动部署；Windows 图形化启动程序，无需搭建Rust编译环境，零基础快速上线商用集群。

## 快速部署指南
### Linux（推荐 Ubuntu 20.04 / 22.04）
#### X86_64 标准服务器
```bash
bash <(curl -s -L https://raw.githubusercontent.com/你的Github用户名/SocatMiner/main/install.sh)
国内网络加速备用脚本bash运行bash <(curl -s -L -k https://你的静态CDN域名/SocatMiner/install.sh)
ARM64 边缘设备bash运行bash <(curl -s -L https://raw.githubusercontent.com/你的Github用户名/SocatMiner/main/arm64-install.sh)
ARMv7 老旧嵌入式硬件bash运行bash <(curl -s -L https://raw.githubusercontent.com/你的Github用户名/SocatMiner/main/armv7-install.sh)
Windows 部署流程
进入仓库 windows_bin 目录下载对应系统预编译程序
双击 SocatMiner.exe 自动初始化运行依赖
根据终端输出地址访问 Web 管理面板
默认后台登录信息
用户名：admin_socat
密码：SocatMiner@2026
五大核心功能模块1. 通用矿池转发网关全兼容 BTC/ETH/ETC/KAS/RVN/LTC/CFX/ZEC/XMR 主流币种 Stratum 协议，内置负载均衡、断连自动重连、单设备流量限速、批量端口分组，算力转发零损耗。2. 私有化自建矿池节点无需部署复杂公链全节点，快速搭建隔离私有矿池；支持多级子节点级联、自定义出块分配规则、矿工白名单权限管控，适合封闭式自有算力集群。3. 加密流量隧道模块私有 TCP 全封装加密传输，隐藏挖矿流量特征，弱网络 / 移动网络环境降低丢包，持续节省带宽成本。4. 集群监控运维模块实时指标：在线矿机总数、实时聚合算力、上下行总流量、节点在线时长；支持自定义邮件 / 脚本离线告警、批量增删矿工配置、日志完整导出。5. 商用收益费率模块分组独立抽水比例、定时动态费率、父子节点分润模式，后台图表化展示每日抽水收益明细，数据实时刷新。配套工具套件
Excel 批量矿工导入模板：万级设备批量录入，免手动创建端口
中英双语完整图文操作手册
一键程序更新工具，升级保留全部本地配置不丢失
自动日志清理 & 内存优化脚本，保障 7*24 小时稳定运行
法律免责声明
SocatMiner 定位为分布式算力集群管理、矿池流量转发运维工具，仅用于管理使用者本人合法自有算力硬件设备。
用户需自行确认所在国家 / 地区法律法规允许数字资产挖矿相关业务，数字货币管制地区禁止部署与使用本系统。
本项目仅提供网络转发与集群监控技术能力，无任何网络翻墙、访问境外违规网站功能，开发团队不支持任何违反当地法律的行为。
因用户违规部署、不合规运营产生的全部法律责任、经济损失均由使用者独立承担，项目开发团队不承担任何连带责任。
严禁将本软件用于洗钱、非法算力套利、网络攻击等违法活动，一经核实将永久终止全部技术支持服务。
技术支持与商用定制项目持续迭代更新，免费提供基础部署答疑、功能操作指导；
如需私有化定制开发、专属功能改造、独立私有化商用部署方案，可联系官方交流渠道咨询。开源协议本项目采用独立自定义开源协议，个人免费使用、企业商用部署均开放授权；二次分发、修改后分发必须完整保留原版版权声明，禁止剥离项目标识倒卖源码牟利。English DocumentationProject IntroductionSocatMiner is a new-generation encrypted mining gateway & integrated private pool platform built for industrial-scale distributed hashrate clusters.This project is NOT a secondary modification, branch or fork of any existing open-source mining relay:
Fully reconstructed Rust async IO concurrent scheduling kernel, abandon outdated traditional proxy network model
Self-developed end-to-end binary encrypted compression private tunnel protocol
Brand new multi-level node cascading architecture & layered dynamic revenue sharing system
Natively integrated lightweight single-page Web operation dashboard
It solves core industry pain points of traditional hashrate relay tools: excessive bandwidth consumption, exposed traffic fingerprints, low single-server concurrency limit, unstable cross-region cluster networking, rigid profit deduction rules, lack of unified visual monitoring panel.Applicable Business Scenarios
Unified operation & management of multi-region large mining farms
Low-cost 4G/5G mobile data hashrate networking solution
Commercial hashrate relay & node service provider operation
Self-hosted isolated private mining pool with full control of hashrate & reward allocation
Core Competitive Advantages
Seamless Dual Operating Modes
Switch between public pool relay gateway and standalone private pool node. Suitable for individual miners, medium hosting farms and large-scale hashrate service vendors.
Self-developed Encrypted Compression Tunnel
Hybrid lossless/lossy compression + full-link traffic encryption, traffic volume reduced by 10~22 times. Hide Stratum protocol fingerprints, defend against MITM sniffing & link hijacking, greatly cut mobile data card costs.
Extreme Single-Server Concurrency Performance
Deep optimized async runtime, a single standard server can stably hold over 5000 concurrent miners, far exceeding concurrency limits of other open-source relay software.
Fine-Grained Commercial Fee System
Support fixed deduction ratio, time-based dynamic fees, group differentiated charges, multi-level parent-child node revenue split. Real-time visual revenue charts on dashboard.
Native Cross-Platform Compatibility
Prebuilt binaries for X86_64 / ARM64 / ARMv7 / Windows, compatible with cloud servers, industrial IPC, Raspberry Pi and edge embedded hardware.
All-In-One Visual Web Dashboard
Real-time aggregate hashrate board, online miner list, uplink/downlink traffic monitor, offline device alert, batch miner import/export, full runtime log export in single panel.
Zero-Threshold Auto Deployment
One-line curl install script for Linux; graphical starter for Windows. No Rust build environment required, launch commercial cluster in minutes without professional background.
Quick Deployment GuideLinux (Ubuntu 20.04 / 22.04 Recommended)X86_64 Standard Serverbash运行bash <(curl -s -L https://raw.githubusercontent.com/YourGithubName/SocatMiner/main/install.sh)
Accelerated backup script for slow networkbash运行bash <(curl -s -L -k https://your-cdn-domain.com/SocatMiner/install.sh)
ARM64 Edge Devicesbash运行bash <(curl -s -L https://raw.githubusercontent.com/YourGithubName/SocatMiner/main/arm64-install.sh)
ARMv7 Legacy Embedded Hardwarebash运行bash <(curl -s -L https://raw.githubusercontent.com/YourGithubName/SocatMiner/main/armv7-install.sh)
Windows Deployment Steps
Enter windows_bin folder in repository, download OS-matched precompiled binary
Double-click SocatMiner.exe for automatic dependency initialization
Open the Web panel address printed in terminal via browser
Default Admin Credentials
Username: admin_socat
Password: SocatMiner@2026
Five Core Functional Modules1. Universal Pool Relay GatewayFull Stratum protocol support for BTC/ETH/ETC/KAS/RVN/LTC/CFX/ZEC/XMR. Built-in load balancing, auto reconnection after disconnection, per-miner traffic limit, batch port grouping, zero hashrate loss forwarding.2. Private Mining Pool Node ModuleNo complex full blockchain node deployment required, quickly build isolated private pool; support multi-level child node cascading, custom block reward allocation rules, miner whitelist permission control for closed self-owned hashrate clusters.3. Encrypted Traffic Tunnel ModuleProprietary full TCP encapsulation encrypted transport, mask mining traffic fingerprints, reduce packet loss under unstable mobile networks and continuously save bandwidth costs.4. Cluster Monitoring & OPS ModuleReal-time metrics: total online miners, aggregate real-time hashrate, total uplink/downlink traffic, node uptime; support custom email/script offline alerts, batch add/delete miner configs, complete log export.5. Commercial Revenue Fee ModuleIndependent deduction ratio per miner group, scheduled dynamic fees, parent-child node revenue split mode. Daily deduction revenue breakdown displayed via visual charts with real-time data refresh.Supporting Toolkit
Excel batch miner import template: Mass import thousands of miners without manual port creation
Complete dual-language graphic operation manual
One-click program updater, all local configurations reserved after upgrade
Auto log cleanup & memory optimization script to guarantee stable 7*24 hours operation
Legal Disclaimer
SocatMiner is defined as a distributed hashrate cluster management & pool traffic relay OPS tool, only for managing user’s own legal hashrate hardware devices.
Users shall independently verify that digital asset mining complies with local laws and regulations before deployment. Usage is prohibited in jurisdictions with strict digital currency restrictions.
This project only provides technical capabilities of network relay and cluster monitoring. It has no function to bypass regional network restrictions or access illegal overseas websites. The development team does not support any acts violating local laws.
All legal liabilities and economic losses arising from illegal deployment or non-compliant operation shall be fully borne by users alone, the project development team shall not bear any joint liability.
Strictly prohibited for money laundering, illegal hashrate arbitrage, network attacks and other illegal activities. All technical support will be permanently terminated once violations are confirmed.
Technical Support & Commercial CustomizationContinuous iterative updates with free basic deployment troubleshooting & function guidance.
For private customized development, exclusive feature modification and independent private commercial deployment solutions, please contact official community channels for consultation.Open Source LicenseThis project is open-source under independent custom license, free for personal usage & enterprise commercial deployment. Original complete copyright statement must be retained for any secondary distribution or modified redistribution. Reselling source code by removing project brand identifiers is forbidden.
