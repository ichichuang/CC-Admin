<!--
  @copyright Copyright (c) 2025 chichuang
  @license MIT
  @description cc-early-bird 企业级后台管理框架 - Monorepo 指南
  本文件为 chichuang 原创，禁止擅自删除署名或用于商业用途。
-->

# Monorepo 架构指南

## 📋 概述

early-bird 已成功升级为基于 pnpm Workspace 的 monorepo 架构，实现了多包管理和代码共享。

## 🏗️ 架构结构

```
early-bird/
├── packages/           # 共享包
│   ├── core/          # 核心框架包
│   ├── ui/            # UI组件库包
│   └── types/         # 类型定义包
├── apps/              # 应用包
│   └── admin/         # 主管理后台应用
├── tools/             # 开发工具
└── docs/              # 文档
```

## 📦 包说明

### @cc/early-bird-core

核心框架包，包含：

- **API 管理**: 统一的接口管理和请求封装
- **状态管理**: 基于 Pinia 的状态管理
- **路由管理**: 动态路由和权限控制
- **工具函数**: 通用工具函数和模块加载器

### @cc/early-bird-ui

UI组件库包，包含：

- **通用组件**: 可复用的业务组件
- **布局组件**: 页面布局和导航组件
- **样式系统**: UnoCSS 配置和主题系统

### @cc/early-bird-types

类型定义包，包含：

- **全局类型**: 应用级别的类型定义
- **环境变量类型**: 环境配置的类型定义
- **路由类型**: 路由相关的类型定义
- **用户类型**: 用户相关的类型定义

### @cc/early-bird-app-admin

主管理后台应用，包含：

- **页面视图**: 业务页面和组件
- **应用配置**: 应用特定的配置
- **业务逻辑**: 具体的业务实现

## 🚀 开发命令

### 安装依赖

```bash
pnpm install
```

### 开发模式

```bash
# 启动主应用
pnpm dev

# 启动特定应用
pnpm dev:admin
```

### 构建

```bash
# 构建主应用
pnpm build

# 构建分析
pnpm build:analyze
```

### 代码检查

```bash
# 类型检查
pnpm type-check

# 代码格式化
pnpm format

# 代码检查
pnpm lint
```

## 🔧 包间依赖

### 依赖关系

```
@cc/early-bird-app-admin
├── @cc/early-bird-core
├── @cc/early-bird-ui
└── @cc/early-bird-types

@cc/early-bird-ui
└── @cc/early-bird-core

@cc/early-bird-core
└── @cc/early-bird-types
```

### 导入方式

```typescript
// 导入核心包
import { store, router } from '@cc/early-bird-core'

// 导入UI组件
import { Loading, LayoutAdmin } from '@cc/early-bird-ui'

// 导入类型
import type { UserInfo } from '@cc/early-bird-types'
```

## 📝 开发规范

### 1. 包命名规范

- 使用 `@cc/early-bird-` 前缀
- 包名使用 kebab-case
- 版本号统一管理

### 2. 导出规范

- 每个包必须有 `index.ts` 统一导出
- 使用命名空间避免冲突
- 提供完整的类型定义

### 3. 依赖管理

- 共享依赖放在根目录
- 包特定依赖放在包内
- 使用 `workspace:*` 引用本地包

## 🔄 迁移说明

### 原有功能保持

- ✅ 自动化模块导入机制
- ✅ 统一的目录结构
- ✅ 完整的工具链
- ✅ 开发体验优化

### 新增功能

- ✅ 多包管理
- ✅ 代码共享
- ✅ 独立构建
- ✅ 类型安全

## 🛠️ 故障排除

### 常见问题

1. **模块找不到**
   - 检查包是否正确安装
   - 确认导入路径正确
   - 验证 TypeScript 配置

2. **类型错误**
   - 确保类型包正确导出
   - 检查 tsconfig.json 配置
   - 验证包间依赖关系

3. **构建失败**
   - 清理 node_modules 重新安装
   - 检查 Vite 配置
   - 验证包导出配置

### 调试命令

```bash
# 清理并重新安装
pnpm workspace:clean

# 检查包依赖
pnpm list --depth=0

# 验证工作空间
pnpm why @cc/early-bird-core
```

## 📚 扩展指南

### 添加新包

1. 在 `packages/` 下创建新目录
2. 创建 `package.json` 配置
3. 添加导出入口 `index.ts`
4. 更新工作空间配置

### 添加新应用

1. 在 `apps/` 下创建新目录
2. 配置应用特定的依赖
3. 设置构建和开发脚本
4. 更新根目录脚本

## 🎯 最佳实践

1. **模块化设计**
   - 保持包的单一职责
   - 避免循环依赖
   - 合理划分包边界

2. **类型安全**
   - 提供完整的类型定义
   - 使用 TypeScript 严格模式
   - 避免 any 类型

3. **性能优化**
   - 按需导入组件
   - 优化包大小
   - 合理使用缓存

4. **开发体验**
   - 保持一致的代码风格
   - 提供完整的文档
   - 自动化开发流程
