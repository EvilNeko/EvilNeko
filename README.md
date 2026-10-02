<div align="center">

# 你好，我是 AxisNova 👋

**把东西跑在 Cloudflare 边缘上的人。**

自托管 / Serverless 折腾爱好者，专注于用 Cloudflare Workers 全家桶
把「本来要买台 VPS」的需求变成零成本、免运维的边缘服务。

[![Cloudflare Workers](https://img.shields.io/badge/Cloudflare%20Workers-F38020?style=for-the-badge&logo=cloudflare&logoColor=white)](https://workers.cloudflare.com/)
[![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/docs/Web/JavaScript)
[![Vue](https://img.shields.io/badge/Vue.js-4FC08D?style=for-the-badge&logo=vuedotjs&logoColor=white)](https://vuejs.org/)
[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)

</div>

---

## 🧭 我在做什么

- ☁️ **边缘优先**：能跑在 Workers 上的，就不开服务器。D1 / KV / Durable Objects / R2 按需组合。
- 🤖 **Telegram Bot 工程化**：不只是「能跑」，而是把验签、常量时间比较、降级容错、单元测试都做齐。
- 🔐 **自托管服务**：临时邮箱、密码管理、WebSSH —— 数据留在自己的域名和数据表里。
- 🌐 **网络与代理配置**：分流规则、Cloudflare 优选 IP、订阅转换，把踩过的坑沉淀成配置文件。
- ✍️ **中文文档强迫症**：项目 README 尽可能写清部署步骤，让后来的人少走弯路。

---

## 📌 精选项目

### 🛠 自研

| 项目 | 说明 |
| :--- | :--- |
| **[TGID_bot](https://github.com/EvilNeko/TGID_bot)** | 基于 Cloudflare Workers 的 Telegram ID 与元数据查询机器人。支持群组/频道/论坛话题 ID、回复解析、转发溯源、全量媒体 `file_id` 提取；内置官方 Secret Token 验签、无默认密钥、常量时间比较、UTF-8 字节级截断与 HTML 降级。附 56 个通过用例。 |
| **[ACL4SSR](https://github.com/EvilNeko/ACL4SSR)** | 自用 Clash 分流配置集。含 Mannix 规则集与 No-DNS-Leak 变体，另附一份可定制的 Online Full Custom 模板。 |
| **[fastip](https://github.com/EvilNeko/fastip)** | 自用 Cloudflare 优选 IP 成果：全量扫描结果 `full_ips.txt` 与优选清单 `best_ips.txt`。 |

### 🔧 二次开发 / 自部署改造

> 以下项目基于上游开源仓库修改，用于自己的生产部署，主要动的是安全加固、部署体验与本地化。

| 项目 | 上游 | 改造方向 |
| :--- | :--- | :--- |
| **[AxisNetWork](https://github.com/EvilNeko/AxisNetWork)** | `cmliu/edgetunnel` | 在 VLESS 配置信息中补充显示转换后的订阅内容，便于直接导入 Clash / Sing-box 等客户端。 |
| **[nodewarden](https://github.com/EvilNeko/nodewarden)** | `shuaiplus/nodewarden` | Bitwarden 兼容服务端，运行在 Cloudflare Workers 上。 |
| **[vmail](https://github.com/EvilNeko/vmail)** | `oiov/vmail` | 单域名部署临时邮箱到 Worker，支持收发信、多域名后缀、密码找回与开放 API，D1 存储。 |
| **[CF-Workers-WebSSH](https://github.com/EvilNeko/CF-Workers-WebSSH)** | `cmliu/CF-Workers-WebSSH` | 纯 TypeScript 实现的 SSH 2.0 客户端，借 Durable Objects 直连公网 SSH，前端 xterm.js。 |
| **[TGbot-D1](https://github.com/EvilNeko/TGbot-D1)** | `moistrr/TGbot-D1` | 人机验证、私聊转话题、管理员回复中继、话题名动态更新、关键词自动回复；存储由 KV 迁移到 D1。 |
| **[WorkersAI2API](https://github.com/EvilNeko/WorkersAI2API)** | — | Workers AI → OpenAI 兼容接口，多账号负载均衡 + 可视化管理面板。 |

---

## 🧰 技术栈

**运行时与平台**

![Cloudflare Workers](https://img.shields.io/badge/Workers-F38020?style=flat-square&logo=cloudflare&logoColor=white)
![Cloudflare Pages](https://img.shields.io/badge/Pages-F38020?style=flat-square&logo=cloudflare&logoColor=white)
![D1 (SQLite)](https://img.shields.io/badge/D1-003B57?style=flat-square&logo=sqlite&logoColor=white)
![KV](https://img.shields.io/badge/KV-0051C3?style=flat-square)
![Durable Objects](https://img.shields.io/badge/Durable%20Objects-0051C3?style=flat-square)
![Wrangler](https://img.shields.io/badge/Wrangler-F38020?style=flat-square&logo=cloudflare&logoColor=white)

**语言**

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=flat-square&logo=kotlin&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white)

**Web 与其他**

![Vue](https://img.shields.io/badge/Vue.js-4FC08D?style=flat-square&logo=vuedotjs&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white)
![Telegram Bot API](https://img.shields.io/badge/Telegram%20Bot%20API-2CA5E0?style=flat-square&logo=telegram&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

---

## 📊 GitHub 数据

<div align="center">

[![Followers](https://img.shields.io/github/followers/EvilNeko?style=flat-square&label=Followers&logo=github&color=1f6feb)](https://github.com/EvilNeko?tab=followers)
[![Total Stars](https://img.shields.io/github/stars/EvilNeko?affiliations=OWNER&style=flat-square&label=%E6%94%B6%E8%8E%B7%E6%98%9F%E6%A0%87&logo=github&color=e3b341)](https://github.com/EvilNeko?tab=repositories)
[![Public Repos](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fapi.github.com%2Fusers%2FEvilNeko&query=%24.public_repos&style=flat-square&label=%E5%85%AC%E5%BC%80%E4%BB%93%E5%BA%93&logo=github&color=3fb950)](https://github.com/EvilNeko?tab=repositories)
[![Last Commit](https://img.shields.io/github/last-commit/EvilNeko/TGID_bot?style=flat-square&label=TGID_bot%20%E6%9C%80%E8%BF%91%E6%8F%90%E4%BA%A4&color=8957e5)](https://github.com/EvilNeko/TGID_bot/commits)

<br />

<img width="100%" src="https://ghchart.rshah.org/409ba5/EvilNeko" alt="EvilNeko 的 GitHub 贡献图" />

</div>

> 统计卡片选用 shields.io 与 ghchart，它们在直连网络下也能正常加载；
> `github-readme-stats` 等 `*.vercel.app` 服务在部分网络下不可达，故未采用。

---

<div align="center">

**「能不开服务器，就不开服务器。」**

<sub>如果我的某个项目帮到了你，给个 ⭐ 是最好的鼓励。</sub>

</div>
