# 辩论战术板 · Debate Tactical Board

单文件、零依赖的无限画布辩论备赛工具（中文 / English 双语界面）。
A single-file, zero-dependency, infinite-canvas debate preparation whiteboard (Chinese / English UI).

> ⚠️ **风险提示 / Risk Warning**
>
> **费用风险**：AI 整理功能会调用第三方大模型 API（OpenAI 兼容接口），按调用量 / Token 计费。输入 API Key 并开始整理即会产生真实费用，请自行评估并承担全部费用风险。
>
> **本地泄漏风险**：API Key 保存在浏览器 localStorage 中（与网页版教练共用同一组键），仅存于本机浏览器。但任何本地存储都不是绝对安全的——请勿在公用 / 共享设备上使用，避免 Key 出现在截图与日志中，并定期更换 Key。
>
> **Cost risk**: The AI Organize feature calls third-party LLM APIs (OpenAI-compatible), billed by usage / tokens. Entering an API key and starting an organize run incurs real charges; you are solely responsible for all costs.
>
> **Local leak risk**: Your API key is stored in browser localStorage (shared with the web coach under the same keys), local to this browser only. Still, no local storage is absolutely safe — avoid shared/public devices, keep the key out of screenshots and logs, and rotate it regularly.

## 项目简介 / About

辩论战术板（Debate Tactical Board）是一份用于辩论备赛的无限画布工具：卡片式论点结构、语义连线、自由批注与图形，内置《辩论筑基》体系的备赛体检与 AI 整理。母版为单个 HTML 文件，可直接在浏览器打开，也可封装为安卓 APK 或作为移动网页应用使用。

Debate Tactical Board is an infinite-canvas tool for debate preparation: card-based argument structures, semantic links, free annotations and shapes, plus a readiness check and AI organizing built on the Debate Universal Grammar system. The master is a single HTML file that runs directly in the browser, and can also be packaged as an Android APK or used as a mobile web app.

## 功能特性 / Features

- 无限画布：平移 / 缩放 / 框选（左→右=完全包含，右→左=碰撞选择）/ 多选
- 卡片体系：17 种类型（辩题、定义、讨论范围、标准 B0、分论点、论据、推论、价值点、对方论点、反驳、消化、反转、主线、战术·环节、需根解损、备注），辩位（一~四辩 / 自定义）、时长（MM:SS）、标签、颜色、宽度可调
- 连线：7 种语义类型、4 种箭头状态、实线 / 虚线、悬停 0.3 秒自动连线
- 自由文本、矩形 / 椭圆 / 直线图形
- 剪贴板：Ctrl+C/X/V、Ctrl+A 全选、就地复制、批量操作
- 撤销 / 重做、搜索、类型与辩位筛选、多白板管理、自动本地保存
- 备赛体检：A1→A7 门禁、三种反驳路径覆盖、辩位覆盖、孤立卡片检查
- AI 整理：立论整理 / 攻防查漏 / 结构诊断 / 自由整理（SSE 流式输出、记录留档）
- 导出：PNG 图片、Markdown 辩案、JSON 备份与导入（桌面直接下载；手机系统分享；APK 原生文件保存）

- Infinite canvas: pan / zoom / marquee (left→right = fully contained, right→left = any intersection) / multi-select
- Cards: 17 types (Motion, Definition, Scope of Discussion, Criterion B0, Sub-Argument, Evidence, Inference, Value Point, Opponent Argument, Rebuttal, Absorption, Reversal, Mainline, Tactic·Segment, Need/Inherency/Solvency/Cost-Benefit, Note), speaker role (1st–4th / custom), duration (MM:SS), tags, colors, resizable width
- Links: 7 semantic types, 4 arrow states, solid / dashed, 0.3s hold-to-link
- Free text, rectangle / ellipse / line shapes
- Clipboard: Ctrl+C/X/V, Ctrl+A select-all, duplicate, batch operations
- Undo / redo, search, type & role filters, multi-board management, auto-save to localStorage
- Prep check: A1→A7 gates, three rebuttal-path coverage, role coverage, orphan-card detection
- AI organize: case organize / clash audit / structure diagnosis / custom (SSE streaming, records kept)
- Export: PNG, Markdown brief, JSON backup & import (direct download on desktop; system share on mobile; native file save inside APK)

## 使用方法 / Usage

1. 用浏览器打开 `debate-tactical-board.html`（默认中文，右上角按钮可切换 EN）。
2. 双击空白处新建卡片；把一张卡拖到另一张卡上停留 0.3 秒自动连线。
3. AI 整理：点击工具栏「AI」，填入 API Key / URL / 模型名（与网页版教练共用设置），选择模式后开始整理。

1. Open `debate-tactical-board.html` in a browser (Chinese by default; switch to EN via the top-right button).
2. Double-click empty space to create a card; hold a card on another card for 0.3s to auto-link.
3. AI Organize: click "AI" in the toolbar, enter API Key / URL / model (shared settings with the web coach), pick a mode and start.

## 环境与兼容 / Compatibility

- 桌面：Chrome / Edge / Firefox
- 移动：Android / iOS 浏览器；可封装为 Capacitor APK（内置原生导出通道）
- 数据：localStorage 自动保存；JSON 可完整备份与迁移

- Desktop: Chrome / Edge / Firefox
- Mobile: Android / iOS browsers; packageable as a Capacitor APK (native export channel included)
- Data: auto-saved to localStorage; JSON supports full backup & migration

## 许可 / License

CC BY-NC-SA 4.0（署名-非商业性使用-相同方式共享）。知识体系基于《辩论筑基》（精靈Moon，2020 版 + 2023 Pro 版）。
本工具仅供技术学习使用；AI 输出内容仅供参考，知识准确性以《辩论筑基》官方课程为准。

CC BY-NC-SA 4.0 (Attribution-NonCommercial-ShareAlike). Built on the Debate Universal Grammar system by Moon (2020 + 2023 Pro editions).
For technical learning only; AI-generated output is for reference only — the official DUG video course remains authoritative.