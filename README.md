# 🗂️ ChatGPT历史记录导出器 (ChatGPT Universal Exporter Enhanced)

> 一键导出 ChatGPT 所有聊天记录（支持 JSON / Markdown / HTML 格式），并自动打包为 ZIP 文件保存本地。

---

## 🚀 功能简介

- ✅ 自动批量导出所有对话（包括归档记录）  
- ✅ 支持多种格式（JSON、Markdown、HTML）  
- ✅ 自动生成美观的 HTML 页面（含代码高亮）  
- ✅ 支持团队空间 (ChatGPT Team / Enterprise)  
- ✅ 导出过程带有重试机制，防止中断  
- ✅ 一键打包成 ZIP 文件下载  

---

## 🧩 安装方法

### 1️⃣ 安装 Tampermonkey（油猴插件）

根据浏览器选择安装：
- Chrome / Edge 👉 [https://tampermonkey.net/?ext=dhdg&browser=chrome](https://tampermonkey.net/?ext=dhdg&browser=chrome)
- Firefox 👉 [https://tampermonkey.net/?ext=dhdg&browser=firefox](https://tampermonkey.net/?ext=dhdg&browser=firefox)

安装完成后，浏览器右上角会出现 🐒 图标。

---

### 2️⃣ 安装脚本

👉 **[点此一键安装脚本](https://raw.githubusercontent.com/zjt666666zjt/Chatpt_Exporter/main/chatgpt-exporter.user.js)**  

或手动安装：

1. 打开此仓库中的  
   [`chatgpt-exporter.user.js`](https://github.com/zjt666666zjt/Chatpt_Exporter/blob/main/chatgpt-exporter.user.js)  
2. 点击「Raw」或「原始文件」按钮  
3. 浏览器会自动触发 Tampermonkey 安装提示 → 点击「安装」即可  

---

## 💬 使用说明

1. 登录 [ChatGPT](https://chat.openai.com) 或 [chatgpt.com](https://chatgpt.com)  
2. 等待页面加载后，右下角会出现绿色按钮「Export Conversations」  
3. 点击按钮，选择导出格式（JSON / Markdown / HTML）  
4. 选择导出空间：  
   - 个人空间 → 适用于普通账号  
   - 团队空间 → 适用于 ChatGPT Team / Enterprise 账号  
5. 点击「开始导出」即可，脚本会自动打包下载 ZIP 文件。  

---

## 📦 导出文件结构示例

<pre>
ChatGPT_backup_2025-11-05.zip
├── 对话A_xxx.json
├── 对话A_xxx.md
├── 对话A_xxx.html
├── 对话B_xxx.md
├── Project_工作项目1/
│   ├── 对话1_项目相关.md
│   ├── 对话2_调试记录.html
│
└── Project_学习笔记/
    ├── AI原理研究.md
    └── AI原理研究.html
</pre>

### 💬 文件说明
| 文件类型 | 说明 |
|-----------|------|
| `.json` | ChatGPT 原始对话数据（完整结构） |
| `.md` | Markdown 格式，适合笔记或导入 Obsidian |
| `.html` | 网页格式，带样式与代码高亮 |
| 文件夹名 | 对应 ChatGPT 的“项目 (Project)”名称 |

---

## 🖼️ 导出效果预览

左侧为 Markdown，右侧为导出的 HTML 效果：

![导出效果预览](https://github.com/zjt666666zjt/Chatpt_Exporter/raw/main/preview.png)

---

## ⚠️ 注意事项

- 请确保已登录 ChatGPT，否则脚本无法获取会话数据  
- 导出前可先打开任意一个聊天页面确保 Access Token 可用  
- 若导出失败，可刷新页面重试  
- 所有数据均导出到你的本地，不会上传到任何服务器  

---

## 📜 许可协议

本项目遵循 **MIT License** ，可自由使用、修改、分发。  
> Copyright © 2025  
> 原始脚本作者：Alex Mercer, Hanashiro, WenDavid  

---

## 💡 建议

如果本项目对你有帮助，欢迎：
- 🌟 Star 支持  
- 🐛 提交 Issue 反馈问题  
- 🔄 Fork 项目制作你的定制版本
