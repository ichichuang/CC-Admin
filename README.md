<!--
  Copyright (c) 2025 chichuang
  Licensed under Custom (Non-Commercial Use Only)
-->

# CC-Admin

CC-Admin 企业级后台管理框架 - 基于 Vue 3.5+ 和 TypeScript 5+ 的现代化企业级后台管理框架

## 🚀 特性

- **现代技术栈**: Vue 3.5+ 和 TypeScript 5+
- **原子化CSS**: 使用 UnoCSS 进行样式管理
- **响应式设计**: 支持多端适配
- **国际化支持**: 多语言切换
- **权限管理**: 基于角色的权限控制系统
- **数据可视化**: 丰富的图表组件
- **开发工具链**: 完善的开发工具链

## 📦 技术栈

| 技术       | 版本 | 说明                     |
| ---------- | ---- | ------------------------ |
| Vue        | 3.5+ | 渐进式JavaScript框架     |
| TypeScript | 5+   | 类型安全的JavaScript超集 |
| Vite       | 7+   | 下一代前端构建工具       |
| UnoCSS     | 66+  | 原子化CSS引擎            |
| Pinia      | 3+   | Vue状态管理库            |
| Vue Router | 4+   | Vue官方路由管理器        |
| Alova      | 3+   | 轻量级请求策略库         |

## 🏗️ 核心架构

- **状态管理**: Pinia + pinia-plugin-persistedstate
- **路由系统**: Vue Router 4+
- **HTTP客户端**: Alova (现代化的请求库)
- **样式方案**: UnoCSS (原子化CSS + Tailwind兼容)
- **包管理**: pnpm (性能优先、磁盘友好)
- **代码质量**: ESLint 9+ + Prettier + TypeScript ESLint

## 📁 项目结构

```
cc-admin/
├── src/
│   ├── api/           # API管理 (自动导入)
│   ├── stores/        # 状态管理 (Pinia)
│   ├── router/        # 路由管理 (自动导入)
│   ├── hooks/         # 组合式函数
│   ├── common/        # 公共模块 (自动导入)
│   ├── layouts/       # 布局组件 (admin/screen/fullscreen)
│   ├── views/         # 页面组件
│   ├── components/    # 通用组件
│   └── utils/         # 工具函数
├── docs/              # 项目文档
├── scripts/           # 构建脚本
└── unocss/           # UnoCSS配置
```

## 🚀 快速开始

### 环境要求

- Node.js >= 22.x
- pnpm >= 8.0.0

### 安装依赖

```bash
# 安装依赖
pnpm install
```

### 开发模式

```bash
# 启动开发服务器
pnpm dev
```

### 构建生产版本

```bash
# 构建生产版本
pnpm build

# 预览构建结果
pnpm preview
```

## 📚 文档导航

- [📖 主文档](./docs/README.md) - 完整的项目介绍和使用指南
- [🧩 组件文档](./docs/components/README.md) - 组件使用指南和API文档
- [🔌 API文档](./docs/api/README.md) - API接口文档和最佳实践
- [🛣️ 路由文档](./docs/router/README.md) - 路由配置和权限控制
- [📊 状态管理](./docs/stores/README.md) - Pinia状态管理指南
- [🎨 样式指南](./docs/styles/README.md) - UnoCSS样式系统
- [⚙️ 开发规范](./docs/development/README.md) - 开发规范和最佳实践

## 🎨 设计系统

- **主题系统**: 深色/浅色模式 + 5种功能色系
- **尺寸系统**: 三种预设 + 动态布局尺寸
- **响应式**: 移动端适配 + 多分辨率支持
- **无障碍**: WCAG 2.1 AA级别标准

## 🤝 贡献指南

请查看 [贡献指南](./docs/development/README.md) 了解如何参与项目开发。

## 📄 许可证

本项目采用自定义商业限制许可证，仅供非商业用途使用。

## 🔗 相关链接

- [GitHub 仓库](https://github.com/ichichuang/CC-Admin)
- [在线演示](https://cc-admin-demo.vercel.app)
- [更新日志](./CHANGELOG.md)
