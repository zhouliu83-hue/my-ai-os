# 周正 AI 人格操作系统 (AI Personality OS)

> 版本：2.0 | 格式：纯 Markdown | 兼容：所有主流 LLM
> 原则：可移植 · 可进化 · 人格核心 · 可商业化

## 这是什么

这不是普通的知识库。这是**周正的个人 AI 操作系统**。

目标：构建一个第二大脑，能够——
- 像周正一样思考
- 像周正一样决策
- 像周正一样表达
- 持续学习与进化
- 长期保存认知
- 具备商业复用价值

## 系统结构

```
my-ai-os/
├── 0_system/          # 系统规则与协议
├── 1_identity/        # 人格与身份
├── 2_cognition/       # 思维与认知
├── 3_behavior/        # 行为与执行
├── 4_expression/      # 表达与创作
├── 5_business/        # 商业与变现
├── 6_memory/          # 记忆与经验
├── 7_ai_training/     # AI 训练数据
├── 8_contexts/        # 上下文管理
├── 9_meta/            # 元数据与进化
└── AI_START.md        # AI 读取入口
```

## 核心原则

- **记录推理，而非结果** — AI 从推理中学习认知
- **存储决策逻辑** — 每个决策包含情境、假设、选择原因
- **存储负面偏好** — 讨厌什么比喜欢什么更重要
- **模型无关** — 纯 Markdown，兼容所有 AI 模型
- **高信号密度** — 不说废话，不堆概念
- **永远在进化** — 系统永不完成

## 使用方法

1. 所有 AI 进入本仓库，**必须先读取 AI_START.md**
2. 按需读取对应模块文件
3. 持续通过 6_memory/ 和 7_ai_training/ 迭代进化

## 作者

**周正** — 一个见过社会另一面的创业人

## 多平台兼容

本仓库已适配以下 AI 平台，进入即自动识别：

| 平台 | 入口文件 | 状态 |
|------|----------|------|
| **Codex** (OpenAI) | `AGENTS.md` + skills/ | ✅ 原生支持 |
| **Claude Code** (Anthropic) | `CLAUDE.md` | ✅ 自动加载 |
| **WorkBuddy** | `.workbuddy/config.json` + `.workbuddy/rules.md` | ✅ 自动加载 |
### 如何使用

#### 对于 AI Agent 平台
直接 clone 本仓库，AI 会自动识别入口文件。

#### 对于通用 LLM（ChatGPT Web、Gemini 等）
1. 复制 `AGENTS.md` 的内容作为系统提示词
2. 或把整个仓库作为知识库上传

#### Skill 触发
无论哪个平台，以下触发词都有效：
- `/商业诊断` — 商业模式诊断
- `/对标` — 对标分析
- `/内容诊断` — 内容创作诊断
- `/hook` — 开头优化
- `/小红书标题` — 标题公式
- `/AI检测` — AI 特征识别
- `/目标` — 目标清晰化
- `/决策` — 决策系统
- `/action` — 执行力诊断
- `/好问题` — 问题改写

详见 `skills/` 目录。

### 迁移到新平台

如果你用的 AI 不在以上列表中，用本仓库的 Agent 迁移工具：
1. 输入 `/agent迁移` 触发
2. 指定目标平台
3. 自动生成对应格式的入口文件
## dbskill 商业工具箱（完整集成）

本仓库有周正AI 完整商业诊断工具箱。已跑通整个闭环服务59个个人和公司

### 包含内容

- **21 个 Agent Skill**（`dbskill/skills/`）
- **15 个深度知识包**（`dbskill/知识库/Skill知识包/`）— 约 120 万字
- **原子化知识库**（`dbskill/知识库/原子库/`）— 约 450 万字，从 12,307 条推文提炼
- **高频概念词典**（`dbskill/知识库/高频概念词典.md`）
- **路由系统**：`/dbs` 自动判断意图分发到对应 skill
- **构建工具**：CI/CD 自动构建发布
- **多平台支持**：Claude Code 插件市场、Codex、Trae Solo、Cursor

### Skill 完整列表

| Skill | 触发词 | 功能 |
|-------|--------|------|
| `dbs` | /dbs /商业 | 主入口，自动路由 |
| `dbs-diagnosis` | /问诊 | 商业模式诊断 |
| `dbs-benchmark` | /对标 | 对标分析 |
| `dbs-deconstruct` | /拆概念 | 概念拆解 |
| `dbs-content` | /内容诊断 | 内容创作诊断 |
| `dbs-hook` | /hook | 开头优化 |
| `dbs-xhs-title` | /小红书标题 | 标题公式 |
| `dbs-ai-check` | /AI检测 | AI 写作检测 |
| `dbs-goal` | /目标 | 目标清晰化 |
| `dbs-slowisfast` | /慢就是快 | 慢方法诊断 |
| `dbs-action` | /action | 执行力诊断 |
| `dbs-good-question` | /好问题 | 好问题生成器 |
| `dbs-decision` | /决策 | 决策系统 |
| `dbs-learning` | /学习 | 交互式学习 |
| `dbs-chatroom` | /聊天室 | 定向聊天室 |
| `dbs-chatroom-austrian` | /奥派 | 奥派经济学聊天室 |
| `dbs-content-system` | /内容结构化 | 内容结构化系统 |
| `dbs-agent-migration` | /agent迁移 | Agent 工作台迁移 |
| `dbs-save` | /存档 | 存档 |
| `dbs-restore` | /续上 | 恢复 |
| `dbs-report` | /出报告 | 出报告 |
