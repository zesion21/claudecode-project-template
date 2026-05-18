# Claude Code 项目模板

开箱即用的 AI 开发环境，提供标准化的项目结构、专业技能库、开发规范。

## ✨ 特性

| 特性 | 说明 |
|------|------|
| 🛠 MCP 集成 | 预配置 6 个 MCP 服务器（docx、pdf、excel、fetch、web-browsing、ragflow） |
| 🎯 专业技能 | 13 个技能覆盖产品、后端、前端、UI设计、内容创作等领域 |
| 📋 规范先行 | 内置安全、代码质量、开发流程等硬约束，保证交付质量 |
| 📁 标准结构 | 约定式项目目录结构，开箱即用 |
| 🚀 快速上手 | 只需修改 `CLAUDE.md` 中的占位符即可启动新项目 |

## 🚀 快速开始

### 1. 创建新项目
```bash
# 复制模板目录为你的新项目
cp -r claudecode-project-template your-project
cd your-project
```

### 2. 配置项目
编辑 `CLAUDE.md`，替换所有 `{{ 占位符 }}` 内容：
- 项目名称、类型、描述
- 技术栈信息
- 项目特有约定
- 团队成员信息

### 3. 开始使用
在 Claude Code 中打开项目目录即可使用。

## 📂 目录结构

```
your-project/
├── .claude/
│   ├── settings.json          # Claude Code 配置（MCP服务器等）
│   └── skills/                # 自定义技能库
│       ├── frontend/          # 前端开发技能
│       ├── backend-midway/    # Midway.js 后端技能
│       ├── skills-product-manager/  # 产品经理技能
│       └── ...                # 其他 10+ 专业技能
├── CLAUDE.md                  # 项目配置、规范、技能说明 ⭐ 核心文件
├── README.md                  # 项目说明（给人看的）
└── .gitignore                 # Git 忽略配置
```

## 🎯 可用技能

使用 `/skill 技能名` 调用专业技能：

| 领域 | 技能 | 核心能力 |
|------|------|----------|
| 📊 产品 | skills-product-manager | 需求分析、PRD创作、产品规划、竞品分析 |
| 💻 后端 | backend-midway | Midway.js + TypeScript + SQLite3 后端开发 |
| 💻 后端 | python-pro | Python 后端、数据分析、脚本开发 |
| 💻 后端 | postgresql-designer | 数据库设计、优化、迁移 |
| 🎨 前端 | frontend | Vue 3 + TypeScript + Ant Design Vue 前端开发 |
| 🎨 前端 | uniapp-architect | UniApp 跨平台应用开发 |
| 🎨 前端 | electron | Electron 桌面应用开发 |
| ✨ 设计 | ui-ux-pro-max | 用户体验设计、交互优化、视觉规范 |
| ✨ 设计 | pencil-design | Pencil 原型设计工具集成 |
| 📝 内容 | skills-ppt-designer | 演示文稿、汇报材料设计 |
| 📝 内容 | skills-wechat-article-writer | 公众号文章、技术博客写作 |
| 🔬 领域 | space | 航天、卫星遥感、遥感影像处理 |

## ⚙️ MCP 服务器

| 服务 | 能力 |
|------|------|
| docx-mcp | Word 文档创建、填充、格式转换 |
| ragflow | RAG 知识库检索、语义搜索 |
| pdf-reader | PDF 内容提取、表格识别 |
| fetch | HTTP 网络请求、API 调用 |
| excel | Excel 表格读写、数据处理 |
| web-browsing-mcp | 网页内容提取、元数据解析 |

## 📝 CLAUDE.md 模板使用说明

`CLAUDE.md` 是 Claude Code 的核心配置文件，采用 **YAML Frontmatter + Markdown 正文** 格式。

### Frontmatter 元数据
```yaml
---
project_name: "用户管理系统"
project_type: "Web应用"
tech_stack:
  frontend: "Vue 3 + TypeScript + Ant Design Vue"
  backend: "Midway.js"
  database: "SQLite3"
  other: "Docker"
---
```

### 占位符清单
所有 `{{ }}` 包裹的内容都需要替换：
| 占位符 | 说明 | 示例 |
|--------|------|------|
| `{{ 项目名称 }}` | 项目的正式名称 | 用户管理系统 |
| `{{ 项目类型 }}` | Web应用/移动端/桌面应用等 | Web应用 |
| `{{ 前端技术栈 }}` | 前端技术组合 | Vue 3 + TypeScript + AntDV |
| `{{ 后端技术栈 }}` | 后端技术组合 | Midway.js + TypeScript |
| `{{ 数据库 }}` | 数据库类型 | PostgreSQL 15 |
| `{{ 其他技术 }}` | 其他关键技术 | Docker + Redis + MinIO |
| `{{ 简要描述项目 }}` | 一句话项目描述 | 企业级用户权限管理系统 |
| `{{ 目标用户群体 }}` | 系统使用者 | 企业IT管理员、运营人员 |
| `{{ v1.0.0 }}` | 版本号 | v1.0.0 |
| `{{ 项目根目录 }}` | Git 仓库目录名 | user-management |
| `{{ 在此添加特有约定 }}` | 项目特殊规则 | 优先兼容 Chrome 浏览器 |
| `{{ YYYY-MM-DD }}` | 日期 | 2024-05-18 |
| `{{ 姓名 }}` | 变更人 | 张三 |

### 硬约束说明
`CLAUDE.md` 中定义了 **25+ 条硬约束**，涵盖：
- 🔒 安全约束（敏感信息、SQL注入、XSS防护等）
- 📦 代码质量（TypeScript严格模式、命名规范、错误处理等）
- 🎨 前端约束（组件粒度、状态管理、样式隔离等）
- 🖥️ 后端约束（分层架构、接口规范、数据库设计等）
- 📝 文档约束（接口文档、数据库文档、注释规范等）
- 🧪 测试约束（单元测试、集成测试覆盖要求）

这些约束会被 Claude 读取并在开发过程中自动遵守。

## 🔄 从 OpenCode 迁移说明

本模板由 OpenCode 项目模板迁移而来：

| OpenCode | Claude Code |
|----------|-------------|
| `.opencode` 目录 | `.claude` 目录 |
| `opencode.json` | `.claude/settings.json` |
| `AGENTS.md` | `CLAUDE.md` |

## 📦 兼容性

- ✅ Claude Code CLI
- ✅ Claude Code Desktop
- ✅ Claude Code Web
- ✅ Windows / macOS / Linux

