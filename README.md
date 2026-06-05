# WorkBuddy 使用指南 (workbuddy-guide)

WorkBuddy 全功能使用指南与故障排查手册 —— 一份打包好的 WorkBuddy 参考手册，安装后开箱即用。

## 是什么

一个 WorkBuddy Skill，包含新手学习路径、速查卡片、场景案例、术语表、FAQ 和诊断脚本。当你向 WorkBuddy 询问任何使用问题（连接器配置、专家创建、自动化任务、环境诊断等），它会自动加载这份手册帮你快速定位答案。

## 内容概览

- **新手6步路径** — 立规矩 → 学下指令 → 连工具 → 建专家 → 选模式 → 跑诊断
- **7张速查卡** — MCP故障/专家创建/自动化/前端问题/金融数据/多智能体/新手引导
- **22个场景案例** — 产品经理、运营、HR、开发、财务等真实场景
- **16条FAQ** — 连接器、自动化、专家、记忆、模型等边界问题
- **问题类型决策树** — 先分大类再查关键词，找答案更快
- **术语表** — MCP/RRULE/SOP/Soul.md/模型/网络安全 等核心概念速查
- **诊断脚本** — `check_env.py` 一键环境诊断，`quick-search.sh` 关键词检索

## 安装

1. 在 WorkBuddy 中打开技能市场
2. 搜索 `workbuddy-guide`
3. 点击安装

或从本地导入：

```
将 workbuddy-guide/ 目录放到 ~/.workbuddy/skills/ 下
```

## 使用方式

安装后无需手动触发。当你向 WorkBuddy 提及相关问题时（如"连接器失败了""怎么创建专家""自动化没触发"），Skill 自动加载并提供答案。

也可以用关键词直接问：
- "MCP工具调用失败怎么排查？"
- "Ask和Craft有什么区别？"
- "怎么让AI记住我的偏好？"
- "Auto模型不够好，换哪个？"

## 不适用场景

这份手册是参考工具书，以下情况不适合用它：
- 问版本更新日志的最新内容 → 用 WebFetch 查官方 Changelog
- 需要修改 Skill 文件本身 → 退出 skill，直接让 AI 编辑
- 代码调试 / 编程问题 → 直接描述技术问题
- 创建新 skill → 让 AI 用 Skill 工具直接创建

## 文件结构

```
workbuddy-guide/
├── SKILL.md                         # 技能入口，版本 v1.0.14
├── references/
│   ├── 01-architecture.md           # 核心架构 + 六层定制化体系
│   ├── 02-connector-troubleshooting.md  # 连接器故障排查（含错误码表）
│   ├── 03-expert-workflow.md        # 专家创建修改 + Prompt 设计模式
│   ├── 04-automation-patterns.md    # 自动化配置 + RRULE 模板库
│   ├── 05-quick-cards.md            # 7张速查卡片（含索引）
│   ├── 06-scenario-examples.md      # 22个真实场景案例（含索引）
│   ├── 07-advanced-practice.md      # 进阶工作习惯
│   ├── 08-glossary.md               # 术语表（含模型/网络安全）
│   ├── 09-prompting-best-practices.md  # 提示词最佳实践
│   ├── 10-interaction-modes.md      # 交互模式（Ask/Plan/Craft）
│   ├── 11-memory-system.md          # 三层记忆系统详解
│   ├── 12-faq.md                    # 16条常见问答
│   └── troubleshooting.md           # 跨领域综合诊断决策树
└── scripts/
    ├── check_env.py                 # 一键环境诊断脚本
    └── quick-search.sh              # 知识库关键词检索
```

## 版本

v1.0.14 (2026-06-04)

## 许可

MIT License
