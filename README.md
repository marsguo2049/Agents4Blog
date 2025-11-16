# Agents4Blog - 个人博客写作助手 | Personal Blog Writing Assistant

一个基于智能Agent的博客写作助手系统，帮助用户基于已有资料高效创作优质博客文章。系统集成了内容分析、结构生成和写作辅助等核心功能。

An intelligent Agent-based blog writing assistant system that helps users efficiently create high-quality blog articles based on existing materials. The system integrates content analysis, structure generation, and writing assistance capabilities.

## 🤖 系统 Agent 架构 | System Agent Architecture

### 📊 BlogCategorizer - 内容分类分析Agent | Content Categorization Analysis Agent
**核心能力 | Core Capabilities:** 智能分析和内容规划 | Intelligent Analysis and Content Planning

- 分析现有资料和想法文件（如`ideas.md`）| Analyze existing materials and idea files (e.g., `ideas.md`)
- 自动识别和分类内容主题 | Automatically identify and categorize content topics
- 生成结构化的内容创作计划 | Generate structured content creation plans
- 基于目标受众和优先级进行主题排序 | Prioritize topics based on target audience and importance

**输出报告 | Output Reports:**
- 详细的分类分析报告 | Detailed categorization analysis reports
- 每个主题的核心要点、目标字数、发布优先级 | Key points, target word count, and publication priority for each topic
- 分阶段的创作计划建议 | Phased content creation recommendations

### 🗂️ BlogStructureGenerator - 结构生成Agent | Structure Generation Agent
**核心能力 | Core Capabilities:** 目录结构和文档生成 | Directory Structure and Documentation Generation

- 基于BlogCategorizer分析结果创建文件夹结构 | Create folder structures based on BlogCategorizer analysis results
- 为每个内容类别生成README.md文档 | Generate README.md documentation for each content category
- 创建想法池文件(ideas_pool.md)用于持续收集灵感 | Create ideas pool files (ideas_pool.md) for continuous inspiration collection
- 建立内容模板和索引系统 | Establish content templates and indexing systems

**自动创建的结构 | Automatically Created Structure:**
```
[Category_Folder_Name]/
├── README.md                 # 类别概述和写作指南 | Category overview and writing guide
├── ideas_pool.md            # 持续的想法收集池 | Continuous idea collection pool
├── templates/               # 内容模板（可选）| Content templates (optional)
├── published/               # 已发布文章（可选）| Published articles (optional)
└── drafts/                  # 草稿文章（可选）| Draft articles (optional)
```

## 🎯 核心功能特点 | Core Features

### 智能内容分析 | Intelligent Content Analysis
- **自动分类 | Automatic Categorization**: 基于内容主题智能归类 | Smart classification based on content themes
- **优先级排序 | Priority Sorting**: 根据时效性和重要性排序 | Organize by timeliness and importance
- **受众识别 | Audience Identification**: 精确定位目标读者群体 | Precise target reader group identification
- **创作规划 | Content Planning**: 提供分阶段的内容创作计划 | Provide phased content creation plans

### 结构化内容管理 | Structured Content Management
- **目录组织 | Directory Organization**: 自动创建清晰的文件夹结构 | Automatically create clear folder structures
- **文档生成 | Documentation Generation**: 每个类别配备详细的README指南 | Detailed README guides for each category
- **模板系统 | Template System**: 提供标准化的内容创作模板 | Standardized content creation templates
- **持续优化 | Continuous Optimization**: 支持想法池的持续更新和整理 | Support ongoing updates and organization of idea pools

### 中文本地化支持 | Chinese Localization Support
- **语言适配 | Language Adaptation**: 完全支持中文内容分析和生成 | Full support for Chinese content analysis and generation
- **分类体系 | Categorization System**: 基于中文内容特点的分类系统 | Classification system based on Chinese content characteristics
- **写作指南 | Writing Guidelines**: 针对中文博客的写作规范和建议 | Blog writing standards and suggestions for Chinese content

## 🚀 使用流程 | Usage Workflow

1. **提供素材 | Provide Materials**: 用户上传/输入相关资料和观点 | Users upload/input relevant materials and viewpoints
2. **信息补充 | Information Enhancement**: 系统搜索补充必要背景信息（可选）| System searches for supplementary background information (optional)
3. **角度确认 | Angle Confirmation**: 明确写作角度、目标读者和风格要求 | Clarify writing angle, target audience, and style requirements
4. **协作创作 | Collaborative Creation**: Agent根据用户要求开始写作 | Agents begin writing based on user requirements
5. **迭代优化 | Iterative Optimization**: 基于用户反馈修改和完善文章 | Refine and improve articles based on user feedback

## 📋 系统特点 | System Characteristics

- **用户主导 | User-Driven**: 以用户提供的资料和观点为核心 | Centered on user-provided materials and viewpoints
- **灵活可控 | Flexible & Controllable**: 用户可以随时介入和调整创作方向 | Users can intervene and adjust creative direction at any time
- **轻量高效 | Lightweight & Efficient**: 专注核心功能，避免过度复杂化 | Focus on core functions, avoiding over-complexity
- **风格定制 | Style Customization**: 支持个性化的写作风格和表达方式 | Support for personalized writing styles and expressions

## 🛠️ 技术架构 | Technical Architecture

```
用户输入 → 素材整理 → (可选)信息补充 → 写作执行 → 内容优化 → 最终文章
User Input → Material Organization → (Optional) Information Enhancement → Writing Execution → Content Optimization → Final Article
```

## 📦 快速开始 | Quick Start

```bash
# 安装依赖 | Install dependencies
pip install -r requirements.txt

# 配置API密钥 | Configure API key
export OPENAI_API_KEY="your-key"

# 启动系统 | Start system
python app.py
```

## 💡 使用示例 | Usage Example

```
用户 | User: 我要写一篇关于远程工作效率的文章 | I want to write an article about remote work productivity
      主要观点：1) 时间管理更重要 2) 沟通工具选择关键 3) 工作环境设置 | Main points: 1) Time management is more important 2) Communication tool selection is key 3) Work environment setup
      角度：支持远程工作，面向企业管理者 | Angle: Support remote work, targeting enterprise managers
      风格：数据驱动，专业说服力 | Style: Data-driven, professional persuasion

系统 | System: [整理素材 | Organize Materials] → [补充数据 | Supplement Data] → [制定大纲 | Create Outline] → [生成初稿 | Generate Draft] → [优化润色 | Optimize & Polish]
```

---

**专注内容，让创作更简单 | Focus on content, make creation simpler** ✨
