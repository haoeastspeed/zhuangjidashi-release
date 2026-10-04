# 装机大师 · 镜像定制与无人值守部署工具

![version](https://img.shields.io/badge/version-v1.3.0-3a86f0) ![platform](https://img.shields.io/badge/Windows-10%20%2F%2011%20x64-3a86f0) ![license](https://img.shields.io/badge/免费使用-3fb96b) ![update](https://img.shields.io/badge/自动更新-GitHub-8fb8ff)

**产品主页：<https://haoeastspeed.github.io/zhuangjidashi-release/>**

面向个人与装机商的 Windows 系统镜像深度定制工具。采用「离线挂载定制」方式——不修改当前系统、可反复操作、可保存预设，从驱动/补丁集成、组件精简，到无人值守应答、PXE 批量部署与装机后优化，一站式完成专业级系统封装。

---

## 📥 下载

| 版本 | 大小 | 说明 | 下载 |
|---|---|---|---|
| **安装版（推荐）** | 约 5 MB | NSIS 安装，**支持一键自动更新**，需系统内置 WebView2 | [setup.exe](https://github.com/haoeastspeed/zhuangjidashi-release/releases/latest/download/ZhuangJiDaShi_1.3.0_x64-setup.exe) |
| **便携版** | 约 24 MB | 单 exe 免安装，适合 U 盘携带，需系统内置 WebView2 | [portable.exe](https://github.com/haoeastspeed/zhuangjidashi-release/releases/latest/download/ZhuangJiDaShi_1.3.0_portable.exe) |
| **单文件在线版** | 约 25 MB | 内置 WebView2 引导器，缺少运行时自动联网下载 | [online.exe](https://github.com/haoeastspeed/zhuangjidashi-release/releases/latest/download/ZhuangJiDaShi_1.3.0_online.exe) |
| **单文件离线版** | 约 264 MB | 内置固定 WebView2 运行时，任意机器可直接运行 | [offline.exe](https://github.com/haoeastspeed/zhuangjidashi-release/releases/latest/download/ZhuangJiDaShi_1.3.0_offline.exe) |

> 全部版本请见 [Releases](https://github.com/haoeastspeed/zhuangjidashi-release/releases)。

---

## ✨ 功能特性

- **离线镜像定制**：挂载 WIM/ESD 后离线操作，不触碰当前系统，改动自动备份、可撤销。
- **驱动批量集成**：递归导入驱动文件夹，内置驱动包库，支持硬件无关镜像。
- **最新补丁集成**：自动识别挂载系统版本，批量集成累积/安全更新，按依赖顺序安装。
- **组件精简向导**：细粒度移除预装应用与可选功能，依赖分析、风险分级、中文说明。
- **无人值守应答**：可视化配置分区/账户/区域/OOBE，实时预览标准 `autounattend.xml`，多套预设。
- **任务序列 · PXE**：图形化编排部署序列，内置 PXE 网络部署与监控，批量装机。
- **启动 U 盘 / ISO**：一键生成 BIOS+UEFI 双引导 ISO、多版本合一 U 盘；ISO 挂载浏览/解包。
- **装机后优化 · 驱动**：87 项流畅性优化，智能检测硬件并从官网获取驱动，内置应急网卡驱动。

## 🚀 快速上手

1. 以**管理员身份**运行，进入「镜像处理 → 挂载管理」。
2. 解包 ISO 或选择 `install.wim`，挂载到空工作目录。
3. 在各功能区集成驱动/补丁、精简组件、定制品牌界面。
4. 在「无人值守」可视化配置并保存 `autounattend.xml`。
5. 回到挂载管理**卸载并提交**，再一键生成 ISO / 制作 U 盘 / PXE 部署。

## 🖥️ 系统要求

- Windows 10 / 11（64 位）
- 管理员权限；安装版/便携版需系统内置 WebView2（缺失请用在线/离线版）
- 建议预留 15 GB 以上工作空间

## 🔄 自动更新

软件内置 Tauri 自动更新，更新清单托管于本仓库，提供 **Releases / GitHub Pages / raw 三通道冗余**。在软件内点击「检查软件更新」即可下载并在重启后完成安装；安装版每次启动也可按需检查。

## 📝 更新日志

### v1.3.0（2026-10-04）

- 打通 GitHub 托管自动更新，三通道冗余。
- 组件精简支持批量勾选一键应用、依赖分析与空间统计。
- 补丁按挂载版本自动识别获取；驱动支持本地检测与导入。
- 无人值守支持导入应答、浏览读取版本名、安装背景与提示定制。
- 新增 ISO 挂载浏览/解包、一键提取 install.wim、按目录一键生成 ISO。
- 修复挂载/解包权限与进度、滚动条遮挡、表格列宽等 UI 与稳定性问题。

---

## ⚠️ 免责声明

本软件为系统管理与封装辅助工具，**不包含任何盗版激活或绕过授权的功能**，请在合法授权的系统与映像上使用。精简组件、修改系统设置存在风险，软件已提供自动备份与撤销能力，建议先在虚拟机中验证；因使用不当造成的后果由使用者自行承担。

## ℹ️ 关于本仓库

本公开仓库仅用于**成品分发、产品主页与自动更新托管**；软件源代码不在此公开。问题与建议请通过 [Issues](https://github.com/haoeastspeed/zhuangjidashi-release/issues) 反馈。
