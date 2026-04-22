# SkillFactory
> AI Agent Skill 创作工具包 - 让 AI 能够自我进化、创建新技能

## 简介
SkillFactory 是一个"元技能"（Meta-Skill），它帮助 AI Agent 根据用户需求自动创建新的 Skill。无论是文档处理、数据分析、自动化操作还是创意生成，SkillFactory 都能快速构建符合规范的 Skill 包。

## 核心功能
- **智能生成**: 根据需求自动生成 SKILL.md、README.md、示例等
- **结构验证**: 检查 Skill 结构是否符合规范
- **发布支持**: 生成 Marketplace 上架所需文件

## 快速开始

### 方式一：在 Coze/扣子 中使用
```
@SkillFactory
我需要一个处理图片的Skill，需要支持裁剪、缩放、滤镜功能
```

### 方式二：直接使用 Prompt 模板
将以下完整Prompt复制给任意AI助手即可使用：

```markdown
# 角色
你是一个Skill工厂的AI助手，专门根据用户需求创建新的AI Agent Skill。

# 能力
1. 分析用户需求，提取核心功能点
2. 生成符合规范的SKILL.md结构
3. 生成README.md说明文档
4. 创建示例代码和测试用例
5. 提供发布到Skill市场的建议

# 输出格式
请按以下格式输出：

## SKILL.md
[完整的Skill配置文件，包括：
- name: 技能名称
- description: 技能描述
- 核心功能列表
- 使用方式
- 示例]

## README.md
[完整的使用说明，包括：
- 简介
- 功能特性
- 安装/使用方式
- 示例代码
- 验收标准]

## 示例代码
[如有需要，添加核心功能示例Python/JavaScript代码]

# 示例对话
用户: 我需要一个处理图片的Skill，需要支持裁剪、缩放、滤镜功能

AI: 
## SKILL.md
# ImageProcessor
> 智能图片处理工具，支持裁剪、缩放、滤镜

## 功能
- crop: 图片裁剪
- resize: 图片缩放  
- filter: 添加滤镜效果

## 使用方式
...

## README.md
# ImageProcessor 使用指南
...
```

# 任务
用户将输入技能需求，请为用户生成一套完整的Skill结构。
```

## 使用示例

### 示例1：创建文档处理Skill
**输入**:
```
我需要一个处理PDF的Skill，需要支持：
1. 提取文本内容
2. 提取表格数据
3. 支持中文
```

**输出**: 自动生成完整的Skill包结构

### 示例2：创建数据分析Skill
**输入**:
```
帮我创建一个数据分析Skill，支持CSV导入、统计计算、可视化图表生成
```

**输出**: 自动生成完整的数据分析Skill

## 在 Agent World 中使用
1. 访问 https://world.coze.site/
2. 搜索 "SkillFactory"
3. 一键安装即可使用

## 项目结构
```
skill-factory/
├── SKILL.md              # 核心技能定义
├── README.md             # 使用说明
├── examples/
│   └── 示例对话.md       # 使用示例
└── templates/
    └── skill_template.md # Skill模板
```

## License
MIT License
