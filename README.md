🚀 YAML Connection Monitor (smaidxing-Toolbox)
A high-fidelity, intelligent network status monitoring tool designed for Windows power users.
一款专为 Windows 极客设计的智能网络连接监测与故障诊断助手。

📖 Introduction / 项目简介
YAML Connection Monitor is an industrial-grade desktop utility that automates the monitoring of proxy states and direct network connectivity. Unlike generic uptime tools, it intelligently parses local configuration files (YAML), performs concurrent health checks, and provides detailed fault diagnostics via modern Windows notifications and Enterprise WeChat (WeCom) push.

YAML 连接恢复监测助手 是一款工业级桌面实用工具，旨在自动化监测代理状态与直连网络环境。不同于普通的网络检测脚本，它能够智能解析本地 YAML 配置文件，执行多线程并发健康检查，并通过 Windows 系统通知及企业微信（WeCom）推送提供详尽的故障诊断建议。

✨ Key Features / 核心特性
📦 Zero-Config YAML Parsing / 零配置智能解析:

Automatically extracts proxy ports and parameters from local YAML configurations.

自动读取并解析本地 YAML 配置文件，实现零手动配置接入。

⚡ Concurrent Detection / 多线程并发探测:

Utilizes ThreadPoolExecutor for simultaneous checks of Proxy, Direct, and Fallback nodes.

基于多线程并发机制，同时探测代理、直连及备用地址，确保毫秒级响应。

🛡️ Intelligent Diagnostics / 智能故障诊断:

Classifies network issues: distinguishes between Local Network failure, Node Timeout, DNS Pollution, or Config errors.

内置智能状态机，精准区分本地断网、节点失效、DNS 污染或配置异常。

🔔 Smart Notifications / 异常防骚扰提醒:

Alerts only on state changes (Fault/Recovered) to avoid notification fatigue.

仅在状态发生变化时触发提醒（异常发生/连接恢复），杜绝通知刷屏。

🎨 Professional GUI & Tray / 工业级 UI 与托盘:

Modern Tabbed interface with real-time logging and system tray integration (Pystray).

现代化的选项卡式界面，支持实时日志滚动及系统托盘静默运行。

🔒 Privacy & Security / 隐私与安全:

Base64 obfuscation for sensitive Webhook keys and secure local logging.

对 Webhook 等敏感密钥进行 Base64 混淆存储，确保个人配置安全。

🛠️ Technical Stack / 技术实现
Language: Python 3.x

GUI: Tkinter + PIL (Pillow) for professional UI.

Concurrency: concurrent.futures for high-performance probing.

Network: Native socket handshake for SOCKS5 and urllib for HTTP/S probes.

Notification: PowerShell Toast Integration (Zero-dependency on Windows).

🚀 Quick Start / 快速开始
Download: Get the latest YAML_Monitor.exe from the Releases page.

Config: Select your YAML file and set the monitoring interval.

Run: Click "Start Monitoring" and minimize to the system tray.

下载: 从 Release 页面下载最新的 YAML_Monitor.exe 单文件版。

配置: 选择你的 YAML 配置文件，设置监测频率。

运行: 点击“开始监测”，随后可最小化至系统托盘静默守护。

🤝 Contribution / 贡献
Welcome to submit Issues or Pull Requests to improve the diagnostic logic or UI styling!
欢迎提交 Issue 或 Pull Request，共同优化诊断逻辑或界面样式！

Developed with ❤️ by smaidxing.
