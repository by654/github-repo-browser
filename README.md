<div align="center">

# 🔍 GitHub 仓库浏览器

**纯前端 · 零后端 · 单文件 · 支持 GitHub Pages 一键部署**

一个可以直接在浏览器中打开、无需安装任何软件、无需搭建服务器的 GitHub 仓库阅读工具。

加载任意仓库链接，即可浏览 Markdown 文件、Release 版本、原文件代码，并支持翻译、深浅色主题、代理切换等功能。

提醒：以下功能介绍仅供参考，请以实际为准

[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![No Build](https://img.shields.io/badge/build-none-brightgreen.svg)](#)
[![Single File](https://img.shields.io/badge/single--file-yes-orange.svg)](#)
[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-ready-success.svg)](#)

</div>

---

## ✨ 亮点

- 🚀 **纯前端实现**：单个 HTML 文件，双击即可在浏览器打开使用
- 🎨 **三种版本可选**：从简约到全能，按需选择
- 📱 **响应式设计**：手机 / 平板 / 电脑均可用，竖屏横屏自动适配
- 🌓 **深浅色主题**：跟随系统或手动切换，偏好本地持久化
- 🔐 **Token 加密存储**：AES-GCM 加密后保存到本机，支持私有仓库
- 🌐 **多代理切换**：GitHub 官方 / jsDelivr / ghproxy 等，应对访问受限
- 🌍 **文档翻译**：支持 Google / MyMemory / DeepL / LibreTranslate
- 📦 **ZIP 打包下载**：一键下载单个或多个分支 / Tag
- 🎯 **GitHub Alerts 原生渲染**：`[!NOTE]`、`[!WARNING]` 等样式 1:1 还原
- 🔗 **仓库内链接自动跳转**：MD 中指向同仓库其他文件的链接可在页面内打开
- 📊 **智能 README 优先**：加载仓库后自动打开根目录 README，与 GitHub 官网逻辑一致

---

## 📦 三种版本对比

仓库提供三个独立版本，均为单文件 HTML，可独立部署。你可以根据使用场景选择最合适的一个。

功能请以实际为准，以下表格仅供参考：

| 功能 | 简约版 | 全能版 | 全能翻译版 |
|---|:---:|:---:|:---:|
| 加载 GitHub 仓库 | ✅ | ✅ | ✅ |
| Markdown 渲染 | ✅ | ✅ | ✅ |
| Release 版本浏览 | ✅ | ✅ | ✅ |
| GitHub Alerts 提示框 | ✅ | ✅ | ✅ |
| 代码高亮 | ✅ | ✅ | ✅ |
| 深浅色主题 | ✅ | ✅ | ✅ |
| Token 加密存储 | ✅ | ✅ | ✅ |
| 剪贴板提取仓库链接 | ✅ | ✅ | ✅ |
| 自动打开 README | ✅ | ✅ | ✅ |
| 文件下载 | ✅ | ✅ | ✅ |
| 文件收藏 | — | ✅ | ✅ |
| 全文搜索 | — | ✅ | ✅ |
| 原文件列表（含文本预览） | — | ✅ | ✅ |
| 文件树视图 | — | ✅ | ✅ |
| 异步加载超长文件列表 | — | ✅ | ✅ |
| 多标签页 | — | ✅ | ✅ |
| TOC 目录大纲 | — | ✅ | ✅ |
| Release 对比 | — | ✅ | ✅ |
| ZIP 打包下载 | — | ✅ | ✅ |
| 代理切换 | — | ✅ | ✅ |
| GitHub Pages 链接 | — | ✅ | ✅ |
| 侧边栏折叠（桌面）/ 抽屉（移动） | — | ✅ | ✅ |
| 快捷键（Ctrl+K / Ctrl+F 等） | — | ✅ | ✅ |
| 命令面板 | — | ✅ | ✅ |
| 自定义字号 / 行距 | — | ✅ | ✅ |
| **文档翻译** | — | — | ✅ |
| **翻译服务商选择** | — | — | ✅ |
| **原文 / 译文双语显示** | — | — | ✅ |

---

## 1️⃣ 简约版 — `minimal.html`

**适用场景**：只想快速查看某个仓库的 README 和 Release，不需要任何多余功能。

**核心特性**

- 输入仓库链接即可加载，支持 `owner/repo` 简写
- 剪贴板一键提取 GitHub 链接（支持从聊天记录、文档中识别）
- Markdown 渲染 + 代码语法高亮 + GitHub Alerts 样式
- Release 列表浏览，附件单独下载
- Token 加密存储，可访问私有仓库
- 深浅色主题切换

**为什么选择它**

- 体积最小，加载最快
- 界面最简洁，没有多余按钮
- 适合嵌入到其他页面，或作为快速查询工具

---

## 2️⃣ 全能版 — `full.html`

**适用场景**：需要长期、深度地使用，把它当作主要的 GitHub 阅读器。

**在简约版基础上新增**

- **原文件列表**：不止 Markdown，任何文本文件（TXT / JS / JSON / YAML / Python 等）都能在页面内直接预览并高亮
- **文件收藏**：星标常用文件，下次访问快速定位
- **全文搜索**：在所有已加载的 Markdown 中搜索关键词，支持深度加载
- **文件树视图**：按目录层级组织文件，仓库大了也不乱
- **异步加载**：超过 80 个文件时自动分批加载，滚动到底部继续加载
- **多标签页**：同时打开多个文件，标签切换无需重新加载
- **TOC 目录大纲**：长文档自动生成目录，滚动时高亮当前位置
- **Release 对比**：选择两个版本，查看提交差异和文件变更
- **ZIP 打包下载**：一键下载当前分支 / 多个分支 / 全部 Tag
- **代理切换**：GitHub / jsDelivr / ghproxy / ghfast 四选一
- **GitHub Pages 链接**：自动识别并显示仓库的 Pages 站点
- **侧边栏折叠**：桌面端可收起，移动端变抽屉，互不遮挡
- **命令面板**：`Ctrl+K` 唤出，输入关键词快速跳转文件或执行操作
- **快捷键**：`/` 聚焦搜索、`j/k` 上下切换、`Esc` 关闭弹窗
- **自定义字号与行距**：保护视力，长文阅读更舒适

**为什么选择它**

- 功能最全面，几乎覆盖所有使用场景
- 快捷键 + 命令面板，效率翻倍
- 桌面端和移动端都有最优体验

---

## 3️⃣ 全能翻译版 — `translate.html`

**适用场景**：经常阅读英文 / 日文等外语仓库文档，需要快速翻译。

**在全能版基础上新增**

- **文档一键翻译**：打开 Markdown 文件后，点击「翻译」按钮即可翻译全文
- **多翻译服务可选**：
  - **Google 翻译**：免费，无需 API Key，可能在某些地区不可用
  - **MyMemory**：免费，匿名用户每天约 5000 字符
  - **DeepL API**：高质量翻译，需要 API Key（免费版每月 50 万字符）
  - **LibreTranslate**：开源方案，可自部署，部分公共实例需要 Key
- **双语 / 仅译文两种模式**：可以选择保留原文对照阅读，或直接替换为译文
- **源语言与目标语言可选**：支持 20+ 种语言，源语言支持自动检测
- **智能翻译范围**：只翻译正文文字，代码块、链接、图片、附件列表保持原样
- **实时进度反馈**：翻译过程中显示进度条和剩余时间估算
- **一键恢复原文**：点击「显示原文」即可回到未翻译状态

**为什么选择它**

- 阅读外语文档不再头疼
- 保留原文对照，技术术语可随时核对
- 多个翻译服务备选，一个不行换另一个

---

## 🚀 快速开始

### 方式一：直接使用（推荐）

1. 下载本仓库中的任意一个 HTML 文件
2. 双击在浏览器中打开
3. 输入 GitHub 仓库链接，例如 `https://github.com/microsoft/vscode`
4. 点击「加载」开始浏览

### 方式二：GitHub Pages 部署

1. Fork 本仓库到你自己的账号
2. 进入仓库 **Settings** → **Pages**
3. **Source** 选择 `Deploy from a branch`，**Branch** 选 `main` / `root`
4. 保存后稍等片刻，访问 `https://你的用户名.github.io/github-repo-browser/`

### 方式三：本地服务器

```bash
# 任选一种
python -m http.server 8000
# 或
npx serve
```

然后访问 `http://localhost:8000/full.html`

---

## 🔑 关于 Token

### 是否需要 Token？

- **只看公开仓库**：不需要。未登录限额 60 次/小时，够个人使用
- **访问私有仓库**：需要。Token 需勾选 `repo` 权限
- **频繁使用 / 深度搜索**：建议填写，限额提升至 5000 次/小时

### 如何获取 Token

1. 打开页面 → 设置 → Token 选项卡
2. 点击「创建 Token」，浏览器会打开 GitHub 页面
3. 勾选需要的权限，生成 Token
4. 复制回页面粘贴，点击「保存」

> 🔒 **安全说明**：Token 使用 AES-GCM 加密后保存在你本机的 `localStorage` 中，不会上传到任何服务器。刷新或关闭页面后仍保留，但清除浏览器数据会丢失。

---

## 🌐 关于代理

当所在地区访问 GitHub 受限或遇到限流时，可以在 **设置 → 代理** 中切换：

| 代理 | 说明 |
|---|---|
| **GitHub（默认）** | 官方服务器，最快最可靠 |
| **jsDelivr** | 全球 CDN 镜像，仅公开仓库 |
| **jsDelivr - Gcore** | jsDelivr 备用节点 |
| **ghproxy.net** | 社区代理 |
| **ghfast.top** | 备选社区代理 |

> ⚠️ 代理仅影响 raw 文件（Markdown 内容、图片）的获取，API 请求始终直连 GitHub。

---

## ❓ 常见问题

**Q：为什么输入仓库后提示「速率限制已用完」？**

A：GitHub 对未登录用户限制为 60 次/小时。在设置 → Token 中填写 Token 可提升至 5000 次/小时。

**Q：私有仓库加载失败怎么办？**

A：请确认：① 已在设置中填写 Token；② Token 拥有 `repo` 权限；③ Token 未过期。

**Q：翻译功能一直提示失败？**

A：Google 翻译和 MyMemory 是公开接口，可能受地区限制。建议：① 切换其他翻译服务；② 使用 DeepL 并填写自己的 API Key；③ 检查网络连接。

**Q：ZIP 下载失败怎么办？**

A：ZIP 下载依赖 `codeload.github.com`。如果失败：① 检查网络；② 浏览器可能拦截了自动下载，查看地址栏提示；③ 私有仓库必须填写 Token。

**Q：数据会同步到云端吗？**

A：不会。这是一个纯前端工具，所有数据（Token、收藏、主题偏好、最近记录、翻译配置）都保存在你本机浏览器的 `localStorage` 中，不会上传到任何服务器。

**Q：可以在手机上用吗？**

A：可以。响应式设计已适配手机，竖屏下侧边栏会变成抽屉模式，从左侧滑出，点击遮罩或选中文件后自动收起。

---

## 🛠️ 技术栈

- 纯原生 HTML / CSS / JavaScript，无构建步骤
- [marked](https://github.com/markedjs/marked) — Markdown 解析
- [DOMPurify](https://github.com/cure53/DOMPurify) — XSS 防护
- [highlight.js](https://highlightjs.org/) — 代码语法高亮
- [GitHub REST API](https://docs.github.com/en/rest) — 仓库数据
- [Web Crypto API](https://developer.mozilla.org/en-US/docs/Web/API/Web_Crypto_API) — Token 加密

---

## 📄 许可证

[MIT License](LICENSE) — 可自由使用、修改、分发。

---

## 🙏 致谢

感谢 GitHub 提供的公开 API，以及所有开源依赖的作者。

如果这个工具帮到了你，欢迎给一个 ⭐ Star！

**同时欢迎反馈：173232426@qq.com**
</div>
