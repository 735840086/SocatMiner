SocatMiner
<div align="center"> <a href="#zh-cn">简体中文</a> | <a href="#en">English</a> </div><div align="center">
SocatMiner
High Performance Distributed Mining Cluster Orchestration & Pool Gateway System
<p align="center"> <!-- 主流币种Logo占位，可替换svg/png真实链接 --> <img src="https://via.placeholder.com/48x48/f7931e/000?text=BTC" width="48" alt="Bitcoin"/> <img src="https://via.placeholder.com/48x48/3498db/fff?text=ETH" width="48" alt="Ethereum"/> <img src="https://via.placeholder.com/48x48/168c64/fff?text=ETC" width="48" alt="Ethereum Classic"/> <img src="https://via.placeholder.com/48x48/9146ff/fff?text=RVN" width="48" alt="Ravencoin"/> <img src="https://via.placeholder.com/48x48/f3ba2f/000?text=LTC" width="48" alt="Litecoin"/> <img src="https://via.placeholder.com/48x48/00a3ff/fff?text=KAS" width="48" alt="Kaspa"/> <img src="https://via.placeholder.com/48x48/e84142/fff?text=DOGE" width="48" alt="Dogecoin"/> <img src="https://via.placeholder.com/48x48/292929/fff?text=CFX" width="48" alt="Conflux"/> </p><p align="center"> <!-- 主流矿池Logo占位 --> <img src="https://via.placeholder.com/60x40/06153a/fff?text=F2POOL" width="60" alt="F2Pool"/> <img src="https://via.placeholder.com/60x40/1a1a1a/f7b71c?text=BINANCE" width="60" alt="Binance Pool"/> <img src="https://via.placeholder.com/60x40/222/00b5ff?text=ANTPOOL" width="60" alt="AntPool"/> <img src="https://via.placeholder.com/60x40/000/00cc66?text=BTC.COM" width="60" alt="BTC.com"/> <img src="https://via.placeholder.com/60x40/333/ff6600?text=HIVEON" width="60" alt="Hiveon Pool"/> <img src="https://via.placeholder.com/60x40/111/9933ff?text=EZIL" width="60" alt="Ezil Pool"/> </p><p align="center"> <strong>Not a simple fork / replica — Rebuilt network stack, self-designed encrypted transport protocol, full commercial cluster operation capabilities</strong> </p></div>
简体中文文档
一、项目概述 SocatMiner
SocatMiner 是一套从零底层重构、面向大规模分布式算力集群的商用级矿机网关与私有矿池组网系统。
本项目并非现有开源挖矿转发工具的简单复刻：
重写全链路 IO 并发调度模型
自研二进制加密压缩传输协议
独立设计分层费率、多级节点集群架构
原生集成轻量化 Web 可视化运维面板
专门解决传统挖矿代理存在带宽高、抓包暴露、单机承载低、组网不稳定、抽水规则单一、无统一管控后台等行业痛点，完美适配 4G/5G 流量矿场、异地多节点分布式集群、商用算力中转服务商、私有化自建矿池四大核心业务场景。
二、核心差异化优势
双运行模式架构
矿池流量中转网关 + 私有化私有矿池节点双模式一键切换，个人小规模运维、大型商业矿场、算力服务商均可适配。
自研高强度加密压缩隧道
传输数据内置加密 + 有损无损混合压缩，传输体积缩减 10~22 倍，抵御中间人抓包、链路劫持、流量特征识别，大幅降低流量卡带宽消耗。
超高单机并发承载
底层 Rust 异步 IO 重构，单台普通服务器稳定承载 5000 + 矿机并发在线，远超同类开源转发工具上限。
精细化分层抽水费率系统
支持固定抽水、动态时段费率、分组差异化费率、多级节点分成策略，满足商业化运营灵活收益配置需求。
全平台原生适配
X86_64 / ARM64 / ARMv7 / Windows 全架构预编译二进制，服务器、工控机、边缘嵌入式设备全部兼容。
一体化 Web 可视化管理后台
在线算力监控、设备在线列表、实时流量统计、费率配置、离线告警、运行日志导出、批量端口导入一站式管控。
极简自动化部署
Linux 一键 curl 部署脚本，Windows 图形化启动程序，无需 Rust 编译环境，零基础快速上线商用集群。
三、适用业务场景
多地域分布式大型矿场统一集群管控
自建私有化私有矿池，自主掌控算力与收益规则
4G/5G 流量卡低成本组网矿机集群
跨区域算力中转、算力分发节点服务商运营
批量矿机托管、商用算力代理运营业务
四、快速部署教程
Linux（Ubuntu 20.04 / 22.04 推荐）
X86_64 标准服务器
bash
运行
bash <(curl -s -L https://raw.githubusercontent.com/你的仓库/SocatMiner/main/install.sh)
国内网络备用下载脚本
bash
运行
bash <(curl -s -L -k https://你的静态加速域名/SocatMiner/install.sh)
ARM64 边缘设备（树莓派、工控机）
bash
运行
bash <(curl -s -L https://raw.githubusercontent.com/你的仓库/SocatMiner/main/arm64-install.sh)
ARMv7 老旧嵌入式设备
bash
运行
bash <(curl -s -L https://raw.githubusercontent.com/你的仓库/SocatMiner/main/armv7-install.sh)
Windows 平台部署
进入仓库 windows_bin 目录下载对应系统预编译程序
双击 SocatMiner.exe 自动初始化运行环境
终端输出 Web 后台地址，浏览器打开即可登录管理面板
默认后台账号密码
账号：admin_socat
密码：Miner@2026
五、五大核心功能模块
1. 通用矿池转发网关模块
全兼容 BTC/ETH/ETC/KAS/RVN/LTC/CFX 主流币种 Stratum 协议，支持负载均衡、故障自动重连、单设备流量限速、批量端口分组管理，算力零损耗转发。
2. 私有化自建矿池节点模块
无需复杂链节点配置，快速搭建独立私有矿池，多级子节点级联组网，自定义出块分配规则、矿工权限白名单，适合封闭式自有算力集群。
3. 加密流量隧道模块
自研私有传输协议，TCP 全流量封装加密，屏蔽挖矿特征指纹，弱网络 / 移动网络环境下大幅降低丢包与带宽开销。
4. 集群监控运维模块
实时看板：总在线矿机、实时总算力、上下行流量、节点运行时长；支持设备离线邮件 / 脚本告警、全量运行日志导出、批量删除 / 导入矿工配置。
5. 商业化费率收益模块
分组独立抽水比例、定时动态费率、上下级节点分润模式，后台实时统计每日抽水收益明细，收益数据可视化图表展示。
六、配套辅助工具包
Excel 批量矿工导入模板：万级设备一键批量录入，无需手动添加端口
双语言官方文档：简体中文 / English 完整操作手册
版本自动更新工具：一键检测升级核心程序，保留原有配置不丢失
日志清理 & 性能调优脚本：自动释放内存、清理过期日志，保障长期稳定运行
七、法律与使用免责声明
SocatMiner 定位为分布式算力集群管理与矿池流量转发运维工具，仅用于合法自有算力设备本地集群调度管理。
使用者必须自行确认所在国家 / 地区法律法规允许相关数字资产算力运维业务，严禁在数字货币相关业务管制地区违规使用。
本项目仅提供网络转发、集群监控技术能力，不具备翻墙、访问境外违规网站功能，开发者不鼓励、不支持任何违反当地法律法规的行为。
因使用者违规部署、不合规运营产生的全部法律责任、经济损失由使用者自行全部承担，项目开发团队不承担任何连带责任。
禁止将本项目用于洗钱、非法算力套利、违规网络攻击等违法活动，一经发现永久取消技术支持服务。
八、技术交流 & 商用定制
项目持续迭代更新，免费提供基础部署答疑、功能使用指导；
如需私有化定制开发、专属功能改造、独立商用部署方案，可联系官方技术交流渠道咨询。
九、开源协议
本项目采用独立开源协议开放，允许个人免费使用、企业商用部署；二次分发、二次修改分发需保留本项目原版版权声明，禁止剥离标识倒卖源码盈利。
English Documentation
1. Project Introduction: SocatMiner
SocatMiner is a commercial-grade mining gateway & private pool orchestration system built completely from scratch for large-scale distributed computing clusters.
This project is NOT a simple fork or replica of existing open-source mining relay tools:
Fully rewritten IO concurrent scheduling stack
Self-designed binary encrypted compression transport protocol
Independent layered fee & multi-level node cluster architecture
Natively integrated lightweight Web visual operation panel
It solves long-standing pain points of traditional mining relays: excessive bandwidth consumption, plaintext traffic exposure, low single-machine concurrency limit, unstable cross-region networking, inflexible profit deduction rules, and lack of unified monitoring dashboard.
Scenarios covered: 4G/5G mobile mining farms, multi-location distributed clusters, commercial hashrate relay service providers, self-hosted private mining pools.
2. Core Differentiated Capabilities
Dual Operating Modes
Switch between public pool traffic relay gateway and standalone private mining pool with one click, fit for individual small-scale miners, large commercial farms & hashrate service vendors.
Self-developed Encrypted Compression Tunnel
Built-in end-to-end encryption + hybrid lossless/lossy compression, traffic size reduced by 10~22 times. Defend against MITM sniffing, link hijacking & traffic fingerprint identification, drastically cut mobile data card bandwidth cost.
Extremely High Single Server Concurrency
Rust async IO refactored runtime, a regular single server can stably host over 5000 active miners simultaneously, far exceeding limits of other open-source relay solutions.
Fine-grained Tiered Fee System
Support fixed deduction ratio, time-based dynamic fees, group differentiated charges, multi-level node revenue split policies, fully customizable for commercial profit operation.
Native Cross-Platform Compatibility
Prebuilt binaries for X86_64 / ARM64 / ARMv7 / Windows, compatible with cloud servers, industrial control boards & edge embedded hardware.
All-in-one Visual Web Dashboard
Real-time hashrate monitor, miner online list, traffic statistics, fee configuration, offline alerting, log export & batch port import in single panel.
Zero-threshold Auto Deployment
One-line curl install script for Linux, graphical starter for Windows. No Rust build environment required, launch commercial cluster within minutes.
3. Applicable Business Scenarios
Unified cluster management for multi-region large mining farms
Self-hosted private mining pool with full control over hash & revenue rules
Low-cost 4G/5G mobile network mining cluster deployment
Cross-region hashrate relay & distribution node service operation
Miner hosting & commercial hash proxy service business
4. Quick Deployment Guide
Linux (Ubuntu 20.04 / 22.04 Recommended)
X86_64 Standard Server
bash
运行
bash <(curl -s -L https://raw.githubusercontent.com/YourRepo/SocatMiner/main/install.sh)
Accelerated script for slow network access
bash
运行
bash <(curl -s -L -k https://your-cdn-domain.com/SocatMiner/install.sh)
ARM64 Edge Devices (Raspberry Pi, Industrial IPC)
bash
运行
bash <(curl -s -L https://raw.githubusercontent.com/YourRepo/SocatMiner/main/arm64-install.sh)
ARMv7 Legacy Embedded Hardware
bash
运行
bash <(curl -s -L https://raw.githubusercontent.com/YourRepo/SocatMiner/main/armv7-install.sh)
Windows Deployment
Navigate to windows_bin folder in repository, download precompiled binary matching your OS
Double-click SocatMiner.exe for automatic environment initialization
Access the Web panel URL printed in terminal, log in via browser
Default Admin Credentials
Username: admin_socat
Password: Miner@2026
5. Five Core Functional Modules
1. Universal Pool Relay Gateway
Full Stratum protocol compatibility for BTC/ETH/ETC/KAS/RVN/LTC/CFX. Support load balancing, auto reconnection on failure, per-miner traffic limit, batch port grouping, zero hash loss forwarding.
2. Private Mining Pool Node Module
Deploy independent private pool without complex blockchain node setup. Multi-level child node cascading, custom block reward distribution, miner whitelist permission control for closed self-owned hash clusters.
3. Encrypted Traffic Tunnel Module
Proprietary private transport protocol with full TCP encapsulation & encryption, hide mining traffic fingerprints, reduce packet loss & bandwidth overhead under unstable mobile networks.
4. Cluster Monitoring & OPS Module
Real-time dashboard metrics: total online miners, aggregate hashrate, uplink/downlink traffic, node uptime. Support email/custom script alerts for offline devices, full log export, batch miner config import/delete.
5. Commercial Fee & Revenue Module
Independent deduction ratio per miner group, scheduled dynamic fee, parent-child node revenue split. Dashboard displays daily deduction revenue breakdown with visual charts.
6. Supporting Toolkit
Excel batch miner import template: Mass import thousands of miners without manual port creation
Dual-language official handbook: Complete operation guide in Simplified Chinese & English
Auto version updater: One-click core program upgrade, preserve all existing configurations
Log cleanup & performance tuning script: Auto memory release, expired log purge for long-term stable runtime
7. Legal Disclaimer
SocatMiner is defined as a distributed hash cluster management & pool traffic relay OPS tool, only for scheduling & managing your own legal hash computing devices locally.
Users shall independently verify that digital asset mining operation complies with local laws & regulations in your jurisdiction. Usage is strictly prohibited in regions where digital currency related businesses are regulated or banned.
This project only provides technical capabilities of network relay & cluster monitoring. It has no function to bypass regional network restrictions or access illegal overseas websites. Developers do not encourage or support any acts violating local laws.
All legal liabilities & economic losses arising from illegal deployment or non-compliant operation shall be fully borne by users. The development team shall not bear any joint liability.
This software must not be used for money laundering, illegal hash arbitrage, unauthorized network attacks or other criminal activities. Technical support will be permanently terminated once violations are confirmed.
8. Technical Support & Commercial Customization
Continuous iterative updates with free basic deployment troubleshooting & operation guidance.
For private customized development, exclusive feature modification & dedicated commercial deployment solutions, contact official community channels for consultation.
9. Open Source License
This project is open-source under independent custom license, free for personal usage & commercial enterprise deployment. Original copyright notice must be retained for any secondary distribution or modified redistribution. Reselling source code by removing original branding is forbidden.
