# Yangnb 的工具箱

> 基于 [HackLauncher](https://github.com/) 的绿色便携式安全工具箱,自我整理常用工具,开箱即用。

一个集成了 **120 个常用工具** 的 Windows 安全工具箱,涵盖代理、抓包、扫描器、FUZZ、子域名/指纹、JS 分析、漏洞扫描与利用、框架组件利用、后渗透、代码审计与应急溯源等方向,覆盖渗透测试的完整生命周期。

## 界面预览

![工具箱界面](Snipaste_2026-10-07_09-47-11.png)

## 特性

- 🚀 **开箱即用** —— 基于 HackLauncher 图形化启动器,一键点击启动工具
- 🗂️ **分类清晰** —— 12 个分类,按渗透测试流程组织
- ☕ **环境内置** —— 内置 Java 8 / Java 21 / Python 3.9 运行环境,无需额外配置
- 📦 **绿色便携** —— 解压即用,无需安装
- 🔧 **持续维护** —— 附工具配置备份(`backups/`)与运行日志(`logs/`)

## 环境说明

| 环境 | 路径 | 说明 |
| --- | --- | --- |
| Java 21 | `tools/0_path/jdk-21` | 默认 Java 环境 |
| Java 8 | `tools/0_path/java-8` | 兼容老版本 Java 工具 |
| Python 3.9 | `tools/0_path/Python39` | Python 脚本工具运行环境 |

## 目录结构

```
Yangnb工具箱/
├── HackLauncher-v1.1.7-windows-amd64.exe   # 图形化启动器主程序
├── config.json                             # 工具箱配置(工具/分类/环境)
├── config.db                               # 启动器数据库
├── backups/                                # 配置自动备份
├── logs/                                   # 运行日志
├── tools/                                  # 工具根目录
│   ├── 0_path/                             # Java / Python 运行环境
│   ├── 1_常用/                             # 常用工具
│   ├── 2_微信小程序/                        # 小程序抓包/反编译
│   ├── 3_杂项/                             # 杂项工具
│   ├── 4_redteam/                          # 红队工具
│   │   ├── 1_扫描器/
│   │   ├── 2_FUZZ/
│   │   ├── 3_子域名andcms扫描/
│   │   ├── 4_js/
│   │   ├── 5_漏扫and利用/
│   │   ├── 6_框架and组件/
│   │   └── 7_后渗透/
│   ├── 5_wordlist/                         # 字典库
│   ├── 6_代码审计/                          # 代码审计工具
│   └── 7_溯源/                             # 应急溯源 / 蓝队工具
└── README.md
```

## 工具清单

### 常用(5)

| 工具 | 说明 |
| --- | --- |
| Fclash | 代理客户端 |
| Everything | 极速本地文件搜索 |
| IDM | 下载工具 |
| Yakit | 综合渗透测试平台 |
| BurpSuite | Web 抓包 / 渗透测试 |

### 微信小程序(2)

| 工具 | 说明 |
| --- | --- |
| KillWxapkg | 小程序源码提取 |
| wxapkg | 小程序包反编译 |

### 杂项(5)

| 工具 | 说明 |
| --- | --- |
| 010Editor | 十六进制编辑器 / 隐写分析 |
| DiskInfo64 | 磁盘信息检测 |
| IP 归属批量查询 | IP 归属地批量查询 |
| Wireshark | 网络抓包分析 |
| 图吧工具箱 | 硬件检测工具箱 |

### 扫描器(10)

| 工具 | 说明 |
| --- | --- |
| dddd | 综合漏洞扫描器 |
| fscan | 内网综合扫描 |
| Goby | 资产扫描 / 漏洞探测 |
| masscan | 高速端口扫描 |
| rustscan | 极速端口扫描 |
| Xray | Web 漏洞扫描 |
| yinvulkiller | 综合漏洞扫描 |
| 超级弱口令检查工具 | 弱口令爆破 |
| Fir-Fetch | 漏洞利用辅助 |
| mitan | 指纹识别 / 弱口令扫描 |

### FUZZ(6)

| 工具 | 说明 |
| --- | --- |
| dirsearch | 目录扫描 |
| feroxbuster | 目录扫描 |
| ffuf | 高速 FUZZ |
| gobuster | 目录 / 子域名扫描 |
| PackerFuzzer | 前端打包器漏洞检测 |
| Arjun | HTTP 参数发现 |

### 子域名 & CMS 指纹(4)

| 工具 | 说明 |
| --- | --- |
| ehole | 资产指纹 / CMS 识别 |
| OneForAll | 子域名收集 |
| subfinder | 子域名发现 |
| Layer | 子域名挖掘机 |

### JS 分析(4)

| 工具 | 说明 |
| --- | --- |
| 转子女神 | 小程序反编译 / 辅助 |
| URLFinder | JS 中 URL / 接口提取 |
| jjjjjjjs | JS 信息提取 |
| packjs | 打包器漏洞检测 |

### 漏扫 & 利用(13)

| 工具 | 说明 |
| --- | --- |
| afrog | POC 批量验证 |
| nuclei | 漏洞扫描引擎 |
| commix | 命令注入检测 |
| ds_store_exp | .DS_Store 信息泄露利用 |
| fuxploider | 文件上传漏洞检测 |
| jwt_tool | JWT 令牌测试 |
| spf_fake | SPF 伪造检测 |
| sqlmap | SQL 注入检测 / 利用 |
| SSRFmap | SSRF 检测 / 利用 |
| UploadRanger | 文件上传辅助 |
| XSStrike | XSS 检测 |
| xxe_tool | XXE 检测 |
| ghauri | SQL 注入检测 |

### 框架 & 组件(42)

| 工具 | 说明 |
| --- | --- |
| MYExploit | 综合利用框架 |
| Exp-Tools | 漏洞利用工具集 |
| daydayExp | 漏洞利用工具集 |
| LiqunKit | 漏洞利用工具集 |
| apt_tools | 综合漏洞利用 |
| hyacinth | 综合漏洞利用 |
| DahuaExploitGUI | 大华设备漏洞利用 |
| Rookie | 海康 / 亿赛通通杀 |
| hikvision 漏洞利用工具 | 海康威视漏洞利用 |
| RuoYiExploitGUI | 若依框架漏洞利用 |
| Ruoyi-All | 若依框架漏洞利用 |
| ruoyiVuln | 若依框架漏洞利用 |
| NacosExploit | Nacos 漏洞利用 |
| NacosAddUser | Nacos 添加用户 |
| NacosRce | Nacos RCE |
| NacosExploit_v1.1 | Nacos 内存马 GUI |
| NacosExploitGUI_v4.0 | Nacos 综合利用 GUI |
| OA 解密(DecryptTools) | OA 密码解密 |
| YONYOU-TOOL | 用友漏洞利用 |
| YongYouNcTool | 用友 NC 漏洞利用 |
| 致远 OA 漏洞全版本扫描工具 | 致远 OA 漏洞扫描 |
| TongDaOATools | 通达 OA 漏洞利用 |
| TongdaTools | 通达 OA 漏洞利用 |
| ShiroExploit(飞鸿) | Shiro 反序列化 |
| shiro_attack | Shiro 综合攻击 |
| shiro_tool | Shiro(有 key 无链) |
| SBSCAN | SpringBoot 信息泄露扫描 |
| SpringBoot-Scan | SpringBoot 信息泄露扫描 |
| Spring_All_Reachable | Spring 漏洞利用 |
| XM-SpringExploitGUI | Spring 综合利用 GUI |
| SpringBootExploit | SpringBoot 漏洞利用 |
| Struts2 漏洞检查工具 2018 版 | Struts2 漏洞扫描 |
| Struts2(ABC123) | Struts2 漏洞利用 |
| rexha(ThinkPHP) | ThinkPHP 漏洞利用 |
| TP_Attack_GUI | ThinkPHP 攻击 GUI |
| ThinkPHPLogScan | ThinkPHP 日志扫描 |
| ThinkphpGUI(莲花) | ThinkPHP 漏洞利用 |
| ThinkPHP(gui_tools) | ThinkPHP 漏洞利用 |
| Weblogic-GUI(内存马) | Weblogic 内存马 |
| WeblogicTool_1.3 | Weblogic 漏洞利用 |
| WebLogic 全版本(superman) | Weblogic 漏洞利用 |
| WeblogicVuln(雷石) | Weblogic 漏洞利用 |

### 后渗透(18)

| 工具 | 说明 |
| --- | --- |
| AntSword | 中国蚁剑 |
| caidao | 中国菜刀 |
| 哥斯拉 | Webshell 管理 |
| 冰蝎 | Webshell 管理 |
| 马子 | Webshell 合集 |
| Multiple 数据库综合利用工具 | 数据库综合利用 |
| MDUT 修改版 | 数据库综合利用 |
| oracleShell | Oracle 利用 |
| SQLTOOLS | MSSQL 命令执行 |
| postgreUtil | PostgreSQL 利用 |
| Sylas | 数据库综合利用 |
| RedisDesktopManager | Redis 图形化管理 |
| RedisEXP | Redis 利用 |
| redis-cli | Redis 命令行客户端 |
| Godzilla(原版) | 哥斯拉原版 |
| 冰蝎二开 | 冰蝎二次开发版 |
| 哥斯拉二开 | 哥斯拉二次开发版 |
| 天蝎 | 权限管理工具 |

### 代码审计(1)

| 工具 | 说明 |
| --- | --- |
| Seay 源代码审计系统 | PHP 代码审计 |

### 溯源(10)

| 工具 | 说明 |
| --- | --- |
| 蓝队工具箱 | 蓝队综合工具 |
| D-Eyes | 恶意文件检测 |
| QDoctor | 恶意代码检测 |
| Hawkeye | 恶意文件检测(Yara) |
| whoamifuck | Linux 主机信息采集 |
| LinuxCheck | Linux 应急检查 |
| shell-analyzer | Webshell 分析 |
| hema(河马查杀) | Webshell 查杀 |
| Ddun(D 盾) | Webshell 查杀 |
| 内存马 2 | 内存马检测 / 查杀 |

## 快速开始

1. 克隆或下载本仓库到本地(推荐放到非中文路径,避免个别工具兼容问题);
2. 双击 `HackLauncher-v1.1.7-windows-amd64.exe` 启动;
3. 在左侧分类中选择工具,点击即可运行。

> 💡 部分工具需要在启动器中配置好 Java / Python 环境路径,本仓库已内置在 `tools/0_path/` 中,默认即可使用。

## 免责声明

本工具箱仅供**安全研究与授权测试**使用。使用者需遵守所在国家/地区的法律法规,未经授权对目标系统进行扫描、测试或利用属违法行为,由此产生的一切后果由使用者自行承担,与本项目无关。
