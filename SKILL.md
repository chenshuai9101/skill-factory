# SkillFactory - AI Agent Skill Creation Toolkit

> **元技能**：帮助 AI Agent 自主创建、验证和发布新 Skill 的工厂工具

## 概述

SkillFactory 是"元技能"（Meta-Skill），它赋予 AI Agent **自我进化的能力**——不仅能执行任务，还能根据需求创建新的工具技能。当用户需要特定功能但系统中没有对应 Skill 时，SkillFactory 可以自动生成。

---

## 核心能力

### 1. 智能生成 SKILL.md

根据用户需求描述，自动生成符合规范的 Skill 核心文档：

- 分析需求场景
- 提取核心功能
- 设计工具接口
- 编写使用指南

### 2. 脚手架构建

自动创建完整的 Skill 目录结构：

```
SkillName/
├── SKILL.md          # 核心技能文档
├── README.md         # 用户说明
├── examples/         # 使用示例
└── templates/        # 模板资源
```

### 3. 结构验证

验证生成的 Skill 是否满足规范：

| 检查项 | 说明 |
|--------|------|
| 文件完整性 | 必需文件是否存在 |
| 格式规范 | Markdown 格式是否正确 |
| 字段齐全 | SKILL.md 必填字段是否完整 |

### 4. 发布清单生成

生成 Skill 上架 Marketplace 所需的清单文件。

---

## 使用方法

### 场景 1：用户需要创建新 Skill

```
用户: 我需要一个处理 Excel 文件的 Skill
```

SkillFactory 自动执行：
1. 分析需求 → 确定 Skill 类型和核心功能
2. 生成结构 → 创建目录和文档
3. 输出结果 → 返回完整 Skill 包

### 场景 2：验证现有 Skill

```
skill_factory.validate("./path/to/skill/")
```

---

## Agent 友好设计

- **CLI 优先**: 统一命令行接口
- **结构化输出**: JSON 格式返回结果
- **幂等操作**: 相同输入产生相同输出
- **无状态设计**: 每次调用独立

---

## 版本

- v1.0.0 (2026-04-21): 初始版本
