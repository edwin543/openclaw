# 个人补课清单（Backlog）—— 分享版起点

> **这是分享版起点 backlog**——汇总了"前两节课会触发到的概念"，给你一个**起点清单**。
>
> 真正的 `_backlog.md` 是个人化的——不同学习者熟悉的概念不一样。请把本文件复制到你的项目目录 `docs/learning/_backlog.md` 后，按你自己的吸收情况维护。

---

## 怎么用这个清单

- **状态约定**：
  - ⬜ 未讲解 / 我不熟
  - 🔄 已简单提及，待深入 / 我半懂
  - ✅ 已完整讲解 / 我已掌握（请附笔记链接）
- **平时主线学习不打断**；遇到清单里的概念，AI 会简单一句话带过
- **每讲完一个完整模块**（例如读完一个 extension），抽 5-10 分钟集中补 1-3 个本次相关的盲区
- **补讲完成后**，把状态改成 ✅，并补上笔记链接
- **后续遇到新盲区**，及时追加到本表

> **建议**：拿到这份起点清单后，**先按你自己的水平把状态打一遍**——熟悉的打 ✅，半懂的打 🔄，完全没概念的打 ⬜。这样 AI 后续遇到这些概念时知道该不该展开。

---

## 一、编程语言与工具链

| # | 概念 | 状态 | 引入处 |
|---|------|------|--------|
| 1 | TypeScript（与 JavaScript 的关系，为什么大项目用 TS） | ⬜ | 全景导览 |
| 2 | Node.js 与 npm 生态 | ⬜ | 全景导览 |
| 3 | pnpm workspace（vs npm / yarn workspaces） | ⬜ | 全景导览 |
| 4 | monorepo（单仓库多包，与多仓库的对比） | ⬜ | 全景导览 |
| 5 | Vite（前端构建工具） | ⬜ | 全景导览 |
| 6 | tsdown / Rolldown（TS 打包器） | ⬜ | 全景导览 |
| 7 | oxlint / oxfmt（基于 Rust 的现代 lint/format 工具） | ⬜ | 全景导览 |
| 8 | vitest（测试框架，与 Jest 的关系） | ⬜ | 全景导览 |

## 二、协议与架构概念

| # | 概念 | 状态 | 引入处 |
|---|------|------|--------|
| 9 | Plugin / Extension 架构（软件设计层面的"插件化"） | ✅ | 插件机制解剖 |
| 10 | Code plugin vs Bundle-style plugin（OpenClaw 的两类插件） | 🔄 | 全景导览 |
| 11 | Skill（OpenClaw 里的"技能"概念，与 plugin 的区别） | ✅ | 全景导览 + 插件机制解剖 |
| 12 | MCP（Model Context Protocol） | ⬜ | 全景导览 |
| 13 | ACP（Agent Client Protocol，对应 `src/acp/`） | ⬜ | 全景导览 |
| 14 | Gateway / Control Plane（网关 / 控制平面） | 🔄 | 插件机制解剖 |
| 15 | Sandbox（沙箱：进程级、容器级、语言级） | ⬜ | 全景导览 |
| 16 | Agent / Agent Harness（AI 代理的工程实现） | ⬜ | 全景导览 |
| 17 | Provider 模式 | ✅ | 插件机制解剖 |
| 18 | 控制反转（Inversion of Control, IoC） | 🔄 | 插件机制解剖 |
| 19 | Strategy 模式（与 Provider 模式相关） | 🔄 | 插件机制解剖 |
| 20 | 声明式 vs 命令式（Declarative vs Imperative） | 🔄 | 插件机制解剖 |
| 21 | 关注点分离（Separation of Concerns, SoC） | 🔄 | 插件机制解剖 |
| 22 | 正交设计（Orthogonal Design） | 🔄 | 插件机制解剖 |
| 23 | 懒加载（Lazy Loading） | 🔄 | 插件机制解剖 |
| 24 | 控制信道 vs 内容信道（双信道协议设计原则） | ✅ | 插件机制解剖 |
| 25 | AI 应用工程的第一性原理（确定性核心 + 概率边缘） | ✅ | 插件机制解剖 |

## 三、跨平台与构建

| # | 概念 | 状态 | 引入处 |
|---|------|------|--------|
| 26 | Docker 与容器化基础 | ⬜ | 全景导览 |
| 27 | Gradle 构建（Android） | ⬜ | 全景导览 |
| 28 | Swift / SwiftLint（iOS / macOS 端） | ⬜ | 全景导览 |
| 29 | MLX（Apple Silicon ML 框架，apps/macos-mlx-tts 用到） | ⬜ | 全景导览 |

## 四、工程实践

| # | 概念 | 状态 | 引入处 |
|---|------|------|--------|
| 30 | pre-commit hooks（`.pre-commit-config.yaml`） | ⬜ | 全景导览 |
| 31 | detect-secrets / semgrep（安全扫描工具） | ⬜ | 全景导览 |
| 32 | jscpd（代码重复检测） | ⬜ | 全景导览 |
| 33 | 用日期做 SemVer-like 版本号的策略（CalVer） | ⬜ | 全景导览 |

---

## 跨会话待巩固清单（Cross-session）

随着学习推进，**已讲解但需要在后续多轮中刻意复用以加深记忆**的概念会汇集到这里。

### 当前活跃项（前两节课结束时）

- **控制反转（IoC）** —— 插件机制解剖首次引入；下节课在合适时机刻意复用一次
- **Provider/Strategy 模式** —— 同上
- **控制信道 vs 内容信道** —— 这是个非常通用的架构概念，讲到 `channels/` 模块时可以再复用一次

### 已闭环项 ✅

- ~~Plugin / Extension 与 Skill 的区分~~ —— 通过麦当劳类比建立稳定区分

---

## 与起点清单不同的概念怎么办

后续学习中你一定会遇到本清单**没列**的新概念——AI 会主动补充进来。这是 backlog 的活法：**它一直在长**，不是固定不变的。
