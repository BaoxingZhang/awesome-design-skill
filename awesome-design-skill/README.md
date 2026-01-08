# awesome-design-skill

一个包含 **30+ 专业设计风格提示词**的 Claude Code Skill，可快速应用到 UI/UX 设计和前端开发项目中。

> **免责声明**：本 Skill 中的设计风格提示词来源于 [designprompts.dev](https://www.designprompts.dev/)，由 Twitter/X 用户 [@0xbisc](https://twitter.com/0xbisc) 创建并分享。本项目仅为将这些优秀的设计提示词整理为 Claude Code Skill 格式，以便于在开发工作中使用。所有设计内容的版权归原作者所有。

## 概述

此 Skill 提供了一系列精心策划的设计风格提示词，每种风格都包含：
- 完整的设计指南（颜色、排版、间距、组件等）
- 设计理念和适用场景
- 示例 HTML 文件
- 参考截图

此外，还包含**通用设计原则**和**UI 重构原则**，作为所有设计风格的基础指导。

## 功能特性

- **30+ 设计风格**：涵盖 Monochrome、Bauhaus、Cyberpunk、Material Design 等多种风格
- **设计原则继承机制**：风格特定原则优先，通用原则自动回退
- **完整设计系统**：包含 Design Token、组件样式、布局策略
- **示例代码**：每种风格提供参考 HTML 实现
- **视觉参考**：截图和缩略图便于快速预览

## 安装

将此 Skill 复制到你的 Claude Code skills 目录：

- **用户级别**：`~/.claude/skills/awesome-design-skill/`
- **项目级别**：`.claude/skills/awesome-design-skill/`

## 使用方法

### 基本用法

```
/awesome-design-skill <风格名称>
```

### 示例

```
/awesome-design-skill monochrome
```

执行后，Claude 将：
1. 读取对应风格的完整设计提示词
2. 展示设计风格的参考截图（如有）
3. 参考示例 HTML 文件的实现方式
4. 自动加载通用设计原则作为补充
5. 将设计规范应用到当前任务

### 列出所有风格

```
/awesome-design-skill list
```

### 查看特定风格详情

```
/awesome-design-skill info <风格名称>
```

## 可用设计风格

| # | 风格名称 | 关键词 | 色调 | 描述 |
|---|----------|--------|------|------|
| 1 | Monochrome | `monochrome` | 白 | 极简黑白设计，强调对比度和排版 |
| 2 | Bauhaus | `bauhaus` | 白 | 包豪斯风格，几何形状与原色 |
| 3 | Modern Dark | `modern-dark` | 黑 | 现代深色主题，适合科技产品 |
| 4 | Newsprint | `newsprint` | 白 | 报纸印刷风格，经典排版 |
| 5 | SaaS | `saas` | 白 | SaaS 产品标准设计，清晰专业 |
| 6 | Luxury | `luxury` | 白 | 奢侈品风格，高端优雅 |
| 7 | Terminal | `terminal` | 黑 | 终端/命令行风格，极客审美 |
| 8 | Swiss Minimalist | `swiss-minimalist` | 白 | 瑞士极简主义，网格系统 |
| 9 | Kinetic | `kinetic` | 黑 | 动感设计，运动与能量 |
| 10 | Flat Design | `flat-design` | 白 | 扁平化设计，简洁无阴影 |
| 11 | Art Deco | `art-deco` | 黑 | 装饰艺术风格，几何与奢华 |
| 12 | Material Design | `material-design` | 白 | Google Material 设计规范 |
| 13 | Neo Brutalism | `neo-brutalism` | 白 | 新粗野主义，大胆边框和阴影 |
| 14 | Bold Typography | `bold-typography` | 黑 | 大胆排版，字体为主角 |
| 15 | Academia | `academia` | 白 | 学术风格，经典优雅 |
| 16 | Cyberpunk | `cyberpunk` | 黑 | 赛博朋克，霓虹与未来 |
| 17 | Web3 | `web3` | 黑 | Web3/加密风格，渐变与深色 |
| 18 | Playful Geometric | `playful-geometric` | 白 | 活泼几何，色彩丰富 |
| 19 | Minimal Dark | `minimal-dark` | 黑 | 极简深色，优雅克制 |
| 20 | Claymorphism | `claymorphism` | 白 | 粘土拟物，3D 柔和效果 |
| 21 | Professional | `professional` | 白 | 企业专业风格，稳重可靠 |
| 22 | Botanical | `botanical` | 白 | 植物/自然风格，有机形态 |
| 23 | Vaporwave | `vaporwave` | 黑 | 蒸汽波美学，复古未来 |
| 24 | Enterprise | `enterprise` | 白 | 企业级应用，功能优先 |
| 25 | Sketch | `sketch` | 白 | 手绘草图风格，原型感 |
| 26 | Industrial | `industrial` | 白 | 工业风格，粗犷实用 |
| 27 | Neumorphism | `neumorphism` | 白 | 新拟物主义，柔和凸起效果 |
| 28 | Organic | `organic` | 白 | 有机形态，自然流动 |
| 29 | Maximalism | `maximalism` | 白 | 极繁主义，丰富多彩 |
| 30 | Retro | `retro` | 白 | 复古风格，怀旧美学 |

## 设计原则

本 Skill 包含设计原则指南，作为所有设计风格的基础：

| 原则 | 类型 | 描述 |
|------|------|------|
| General Design Principles | 理论指导 | 布局、层次、一致性、可读性等 10 个通用原则 |
| Refactoring UI Principles | 实战技巧 | 从零开始、层次、间距、色彩等 8 个重构原则 |

**注意**：设计原则会在应用任何设计风格时自动加载，作为风格未指定方面的默认规则。

## 设计原则继承机制

当应用设计风格时，遵循以下优先级：

1. **风格特定原则优先**：风格 prompt.md 中明确指定的规则优先执行
2. **通用原则回退**：风格未提及的方面，使用通用设计原则

示例：
- Monochrome 风格指定"纯黑白、无阴影" → 使用风格特定原则
- Monochrome 未指定"可访问性标准" → 回退到通用原则的 4.5:1 对比度

## 目录结构

```
awesome-design-skill/
├── SKILL.md                    # 主 Skill 文件
├── LICENSE                     # MIT 许可证
├── README.md                   # 本文件
├── screenshots/                # 所有风格截图集中存放
├── thumbnails/                 # 所有风格缩略图
├── principles/                 # 设计原则目录
│   ├── README.md               # 原则索引说明
│   ├── general-design.md       # 通用设计原则（理论指导）
│   └── refactoring-ui.md       # UI 重构原则（实战技巧）
└── design-styles/              # 各风格详细内容
    ├── monochrome/
    │   ├── prompt.md           # 完整设计提示词（含 YAML 元数据）
    │   └── example.html        # 示例 HTML 文件
    └── ... (共 30 个风格)
```

## 注意事项

- 每种风格的提示词来源于 [designprompts.dev](https://www.designprompts.dev/)
- 示例 HTML 文件展示了该风格的典型实现方式，可作为开发参考
- 截图仅作为视觉参考，具体实现请以提示词为准
- 建议根据项目需求选择合适的风格，不要混用冲突的风格

## 致谢

本 Skill 的设计风格内容基于以下来源：

- **[designprompts.dev](https://www.designprompts.dev/)** - 由 [@0xbisc](https://twitter.com/0xbisc) 创建的设计提示词集合
- 感谢原作者分享这些优秀的设计资源

## 许可证

MIT License。详见 [LICENSE](LICENSE)。
