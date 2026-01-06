---
name: Glassmorphism
description: A translucent, frosted glass UI style with blur effects, subtle borders, and layered transparency. Creates a modern, elegant look with depth through glass-like surfaces.
mode: Light
typography: Sans
---

# Glassmorphism Design Style

> 待补充：请从 https://www.designprompts.dev/glassmorphism 复制完整的设计提示词到此文件。

## 临时说明

Glassmorphism（玻璃拟态）是一种现代 UI 设计风格，其核心特征包括：

- **半透明背景**：使用 rgba 或 hsla 颜色实现透明度
- **模糊效果**：backdrop-filter: blur() 创建磨砂玻璃效果
- **微妙边框**：通常使用 1px 的白色半透明边框
- **层叠深度**：通过多层叠加创造深度感
- **柔和阴影**：使用扩散的阴影增强漂浮感

### 典型 CSS 实现

```css
.glass-card {
  background: rgba(255, 255, 255, 0.25);
  backdrop-filter: blur(10px);
  -webkit-backdrop-filter: blur(10px);
  border: 1px solid rgba(255, 255, 255, 0.18);
  border-radius: 16px;
  box-shadow: 0 8px 32px 0 rgba(31, 38, 135, 0.15);
}
```

### 适用场景

- 现代 Web 应用界面
- 移动应用 UI
- 卡片组件
- 导航栏和侧边栏
- 弹窗和模态框

### 设计要点

1. 需要有色彩丰富的背景（渐变或图片）
2. 控制透明度在 0.1-0.4 之间
3. 模糊值通常在 8-20px
4. 边框增强玻璃边缘感
5. 注意浏览器兼容性（Safari 需要 -webkit- 前缀）
