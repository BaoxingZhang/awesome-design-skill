---
name: awesome-design-skill
description: 提供 30+ 专业设计风格提示词，包含完整的 UI 设计规范、示例代码和参考截图
---

# /awesome-design-skill

一个包含 30+ 专业设计风格提示词的集合，可快速应用到 UI/UX 设计和前端开发项目中。

## 概述

此 Skill 提供了一系列精心策划的设计风格提示词，每种风格都包含：
- 完整的设计指南（颜色、排版、间距、组件等）
- 设计理念和适用场景
- 示例 HTML 文件
- 参考截图

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
4. 将设计规范应用到当前任务

### 列出所有风格

```
/awesome-design-skill list
```

### 查看特定风格详情

```
/awesome-design-skill info <风格名称>
```

## 核心指令

当用户调用此 Skill 时，你必须：

1. **解析用户参数**
   - 如果参数是 `list`，显示所有可用风格列表
   - 如果参数是 `info <风格名称>`，显示该风格的详细信息
   - 如果参数是风格名称，加载并应用该风格

2. **加载设计风格**
   - 读取 `design-styles/<风格名称>/prompt.md` 获取设计提示词
   - 读取 `design-styles/<风格名称>/example.html` 获取示例代码
   - 如果存在 `screenshots/<风格名称>.png`，向用户展示参考图

3. **应用设计风格**
   - 将设计提示词作为上下文应用到当前任务
   - 参考示例 HTML 的实现方式
   - 确保生成的代码/设计符合该风格规范

4. **处理无效输入**
   - 如果风格名称不存在，提示用户并显示可用风格列表
   - 如果没有提供参数，询问用户想要使用哪种风格

## 设计风格文件结构

```
awesome-design-skill/
├── SKILL.md                    # 主 Skill 文件
├── screenshots/                # 所有风格截图集中存放（便于预览选择）
│   ├── monochrome.png
│   ├── bauhaus.png
│   ├── modern-dark.png
│   └── ... (以风格名称命名)
└── design-styles/              # 各风格详细内容
    ├── monochrome/
    │   ├── prompt.md           # 完整设计提示词（含 YAML 元数据）
    │   └── example.html        # 示例 HTML 文件
    ├── bauhaus/
    │   ├── prompt.md
    │   └── example.html
    └── ... (共 30 个风格)
```

### prompt.md 元数据格式

每个风格的 `prompt.md` 包含 YAML frontmatter：

```yaml
---
name: Monochrome
description: A stark, editorial design system...
mode: Light        # Light | Dark
typography: Serif  # Sans | Serif | Mono
---
```

## 注意事项

- 每种风格的提示词来源于 https://www.designprompts.dev/
- 示例 HTML 文件展示了该风格的典型实现方式，可作为开发参考
- 截图仅作为视觉参考，具体实现请以提示词为准
- 建议根据项目需求选择合适的风格，不要混用冲突的风格
