<div align="center">

# SocatMiner
## High Performance Distributed Mining Cluster Orchestration & Private Pool Gateway System

<a href="#zh-cn">简体中文</a> · <a href="#en">English</a>

<br>

<!-- 主流虚拟货币图标行 -->
### Supported Coins
<img src="https://via.placeholder.com/48/FF9900/000000?text=BTC" width="48" alt="Bitcoin BTC"/>
<img src="https://via.placeholder.com/48/4E8EE6/FFFFFF?text=ETH" width="48" alt="Ethereum ETH"/>
<img src="https://via.placeholder.com/48/3FB680/FFFFFF?text=ETC" width="48" alt="Ethereum Classic ETC"/>
<img src="https://via.placeholder.com/48/00A4FF/FFFFFF?text=KAS" width="48" alt="Kaspa KAS"/>
<img src="https://via.placeholder.com/48/F2C834/000000?text=LTC" width="48" alt="Litecoin LTC"/>
<img src="https://via.placeholder.com/48/934CFF/FFFFFF?text=RVN" width="48" alt="Ravencoin RVN"/>
<img src="https://via.placeholder.com/48/E84142/FFFFFF?text=DOGE" width="48" alt="Dogecoin DOGE"/>
<img src="https://via.placeholder.com/48/222222/FFFFFF?text=CFX" width="48" alt="Conflux CFX"/>
<img src="https://via.placeholder.com/48/17B2A6/FFFFFF?text=ZEC" width="48" alt="Zcash ZEC"/>
<img src="https://via.placeholder.com/48/8A2BE2/FFFFFF?text=XMR" width="48" alt="Monero XMR"/>

<br>

### Compatible Mining Pools
<img src="https://via.placeholder.com/60x40/051639/FFFFFF?text=F2POOL" width="60" alt="F2Pool"/>
<img src="https://via.placeholder.com/60x40/121212/F7B81C?text=BINANCE" width="60" alt="Binance Pool"/>
<img src="https://via.placeholder.com/60x40/202020/00B4FF?text=ANTPOOL" width="60" alt="AntPool"/>
<img src="https://via.placeholder.com/60x40/000000/00CC66?text=BTC.COM" width="60" alt="BTC.com"/>
<img src="https://via.placeholder.com/60x40/333333/FF6600?text=HIVEON" width="60" alt="Hiveon Pool"/>
<img src="https://via.placeholder.com/60x40/111111/9933FF?text=EZIL" width="60" alt="Ezil Pool"/>
<img src="https://via.placeholder.com/60x40/000000/FF3333?text=NICEHASH" width="60" alt="NiceHash"/>
<img src="https://via.placeholder.com/60x40/1A1A1A/00DDAA?text=WOOLYPOOL" width="60" alt="WoolyPooly"/>

<br>

> **Not a simple fork or replica of any open-source mining relay project**
> Completely reconstructed network IO stack, self-developed encrypted transmission protocol, independent cluster scheduling & tiered revenue architecture for commercial mining operation

</div>

---

<a id="zh-cn"></a>
# 简体中文说明文档
## 一、项目简介
SocatMiner 是一套底层从零重构、面向大规模分布式算力集群的商用级矿机网关与私有矿池组网系统。
本项目绝非同类开源挖矿转发工具的简易复刻，核心底层全部自主研发重构：
- 全新异步IO并发调度模型，抛弃传统老旧转发逻辑
- 自研二进制加密压缩私有传输隧道
- 独立分层费率、多级节点级联集群架构
- 原生轻量化Web可视化运维控制面板

针对性解决传统矿场代理带宽消耗高、算力流量易被抓包识别、单服务器承载量低、异地组网不稳定、抽水收益规则单一、无统一监控后台等行业痛点。
适配四大核心业务场景：4G/5G流量矿场集群、跨地域分布式算力节点、商用算力中转服务商、私有化自建私有矿池。

## 二、核心差异化优势
1. **双模式一体化架构**
一键切换「公矿池流量中转网关」/「私有化独立矿池节点」，个人小规模挖矿、中型托管矿场、商业化算力服务商全部适配。
2. **自研高强度加密压缩隧道**
端到端加密+无损/有损混合压缩算法，传输流量体积压缩10~22倍，屏蔽挖矿流量特征指纹，抵御中间人抓包、链路劫持，大幅降低流量卡带宽成本。
3. **超高单机并发承载上限**
基于Rust底层重构异步运行时，单台普通云服务器可稳定在线承载5000+矿机并发连接，性能远超市面同类开源转发程序。
4. **精细化分层收益费率系统**
支持固定抽水、时段动态费率、矿工分组差异化费率、上下级节点多级分润策略，后台可视化统计每日收益明细，完全适配商业化运营需求。
5. **全平台原生兼容**
提供X86_64 / ARM64 / ARMv7 / Windows 预编译二进制程序，兼容云服务器、工控机、树莓派、嵌入式边缘硬件。
6. **一站式Web可视化运维面板**
实时总算力监控、在线设备列表、上下行流量统计、费率配置、设备离线告警、运行日志导出、批量矿工端口导入，全功能集成无需额外工具。
7. **零门槛自动化部署**
Linux一行curl脚本全自动安装，Windows图形化启动程序，无需搭建Rust编译环境，零基础数分钟完成商用集群上线。

## 三、适用业务场景
- 多地区大型分布式矿场统一集群管控
- 自主搭建私有化私有矿池，完全掌控算力与收益分配规则
- 4G/5G流量卡低成本组网矿机集群运维
- 跨区域算力中转分发、算力节点服务商商业运营
- 批量矿机托管、商用算力代理服务业务

## 四、快速部署教程
### Linux 系统（推荐 Ubuntu 20.04 / 22.04）
#### X86_64 标准云服务器
```bash
bash <(curl -s -L https://raw.githubusercontent.com/你的仓库地址/SocatMiner/main/install.sh)
