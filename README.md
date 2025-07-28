<!--
  @copyright Copyright (c) 2025 chichuang
  @license MIT
  @description CC-Admin 企业级后台管理框架 - README
  本文件为 chichuang 原创，禁止擅自删除署名或用于商业用途。
-->

# CC-Admin 企业级后台管理框架

<p align="center">
  <img src="https://img.shields.io/badge/Vue-3.5+-4FC08D?style=flat&logo=vue.js&logoColor=white" alt="Vue">
  <img src="https://img.shields.io/badge/TypeScript-5+-3178C6?style=flat&logo=typescript&logoColor=white" alt="TypeScript">
  <img src="https://img.shields.io/badge/Vite-7+-646CFF?style=flat&logo=vite&logoColor=white" alt="Vite">
  <img src="https://img.shields.io/badge/UnoCSS-0.66+-333333?style=flat&logo=unocss&logoColor=white" alt="UnoCSS">
  <img src="https://img.shields.io/badge/pnpm-10.12.4-orange?style=flat&logo=pnpm&logoColor=white" alt="pnpm">
</p>

<p align="center">
  基于 Vue 3.5+ 和 TypeScript 5+ 的现代化企业级后台管理框架
</p>

<p align="center">
  <a href="#快速开始">快速开始</a> •
  <a href="#核心特性">核心特性</a> •
  <a href="#技术栈">技术栈</a> •
  <a href="#目录结构">目录结构</a> •
  <a href="#开发指南">开发指南</a> •
  <a href="#代码监控">代码监控</a> •
  <a href="#部署">部署</a> •
  <a href="docs/INDEX.md">📚 文档中心</a>
</p>

---

## 🎯 项目介绍

CC-Admin 是一个现代化的企业级后台管理框架，采用最新的前端技术栈，提供完整的开发工具链和规范化的项目结构。框架致力于为开发者提供高效、可维护、可扩展的管理后台开发体验。**项目严格使用纯 TypeScript，不包含任何 JavaScript 代码。**

### 设计理念

- **📦 模块化设计**: 统一的 `index.ts + modules/` 目录结构
- **🔧 工程化完备**: 完整的代码规范、构建优化、开发调试工具链
- **🎨 现代化UI**: 基于 UnoCSS 的原子化CSS，支持主题切换和响应式设计
- **🌐 国际化支持**: 完整的多语言解决方案
- **🔒 类型安全**: TypeScript 严格模式，完整的类型定义
- **⚡ 开发体验**: 热更新、自动导入、智能提示等现代化开发体验
- **🛡️ 版权保护**: 完整的代码监控和保护系统

---

## 🚀 快速开始

### 环境要求

```bash
Node.js >= 24.3.0
pnpm >= 8.0.0
```

### 安装依赖

```bash
# 克隆项目
git clone <repository-url>
cd cc-admin

# 安装依赖（强制使用 pnpm）
pnpm install
```

### 启动开发

```bash
# 启动开发服务器（同时启动命名规范监听）
pnpm dev

# 构建生产版本
pnpm build

# 预览构建结果
pnpm preview
```

### 开发命令

```bash
# 代码质量检查
pnpm check           # 综合检查（类型+ESLint+命名规范）
pnpm lint            # ESLint 检查并修复
pnpm type-check      # TypeScript 类型检查
pnpm naming-check    # 文件命名规范检查
pnpm naming-watch    # 实时监听文件命名规范

# 代码格式化
pnpm format          # Prettier 格式化

# Git 提交
pnpm commit          # 规范化提交（Commitizen）

# 代码监控
pnpm monitor         # 完整代码监控
pnpm monitor:quick   # 快速代码搜索
```

---

## ✨ 核心特性

### 🏗️ 统一架构设计

- **模块化结构**: 所有功能模块采用 `index.ts + modules/` 统一结构
- **自动导入机制**: 通过 `autoImportModulesSync` 实现模块自动装载
- **类型安全**: 完整的 TypeScript 类型定义和严格模式检查

### 🎨 强大的样式系统

- **UnoCSS 原子化**: 66+ 版本，内置丰富的工具类和快捷方式
- **双主题支持**: 深色/浅色模式无缝切换
- **响应式适配**: 完整的移动端适配和 rem 计算
- **自定义主题**: 灵活的颜色和尺寸配置系统

### 🔧 完整的工具链

- **代码规范**: ESLint + Prettier + 自定义命名规范检查
- **Git 工作流**: Husky + lint-staged + Commitizen 规范化提交
- **构建优化**: Vite 7+ 构建优化、代码分割、性能分析
- **开发体验**: 热更新、路径别名、自动导入、智能提示

### 🌐 国际化系统

- **多语言支持**: 中文简体/繁体、英文等多语言支持
- **智能检测**: 自动检测浏览器语言并应用对应语言包
- **类型安全**: 完整的国际化类型定义
- **动态切换**: 运行时语言切换，无需刷新页面

### 📊 状态管理

- **Pinia 状态管理**: Vue 3 官方推荐的状态管理方案
- **持久化存储**: 自动同步到 localStorage
- **模块化设计**: 按功能模块拆分 Store
- **类型支持**: 完整的类型推导和智能提示

### 🛡️ 代码监控系统

- **版权保护**: 基于独特标识符的精确检测
- **结构分析**: 检测文件组织和模块结构抄袭
- **技术栈识别**: 识别相似的技术栈组合
- **自动监控**: GitHub Actions 定时扫描
- **本地监控**: 支持本地脚本进行详细分析

---

## 🛠️ 技术栈

### 核心框架

| 技术                                          | 版本 | 说明                               |
| --------------------------------------------- | ---- | ---------------------------------- |
| [Vue](https://vuejs.org/)                     | 3.5+ | 渐进式JavaScript框架               |
| [TypeScript](https://www.typescriptlang.org/) | 5+   | JavaScript的超集，提供静态类型检查 |
| [Vite](https://vitejs.dev/)                   | 7+   | 下一代前端构建工具                 |

### 状态管理 & 路由

| 技术                                                                                   | 版本 | 说明               |
| -------------------------------------------------------------------------------------- | ---- | ------------------ |
| [Pinia](https://pinia.vuejs.org/)                                                      | 3+   | Vue 官方状态管理库 |
| [Vue Router](https://router.vuejs.org/)                                                | 4+   | Vue 官方路由管理器 |
| [pinia-plugin-persistedstate](https://github.com/prazdevs/pinia-plugin-persistedstate) | 4+   | Pinia 持久化插件   |

### 网络请求 & 样式

| 技术                                      | 版本  | 说明              |
| ----------------------------------------- | ----- | ----------------- |
| [Alova](https://alova.js.org/)            | 3+    | 现代化请求库      |
| [UnoCSS](https://unocss.dev/)             | 0.66+ | 即时原子化CSS引擎 |
| [Vue I18n](https://vue-i18n.intlify.dev/) | 10+   | Vue 国际化插件    |

### 开发工具

| 技术                                               | 版本 | 说明                   |
| -------------------------------------------------- | ---- | ---------------------- |
| [ESLint](https://eslint.org/)                      | 9+   | JavaScript代码检查工具 |
| [Prettier](https://prettier.io/)                   | 3+   | 代码格式化工具         |
| [Husky](https://typicode.github.io/husky/)         | 9+   | Git hooks 工具         |
| [Commitizen](https://github.com/commitizen/cz-cli) | 4+   | 规范化Git提交工具      |

---

## 📁 目录结构

```
cc-admin/
├── 📁 .cursor/              # Cursor编辑器配置
│   ├── settings.json        # IDE设置
│   ├── cursor-rules         # AI编码规则
│   └── project-rules.md     # 项目规则文档
├── 📁 .github/              # GitHub配置
│   └── workflows/           # GitHub Actions工作流
│       └── cc-admin-monitor.yml # 代码监控工作流
├── 📁 build/                # 构建配置
│   ├── plugins.ts           # Vite插件配置
│   ├── utils.ts             # 构建工具函数
│   └── performance.ts       # 性能优化配置
├── 📁 docs/                 # 项目文档
│   ├── environment-variables.md  # 环境变量说明
│   ├── locale.md            # 国际化文档
│   ├── rem-adapter.md       # 响应式适配文档
│   └── code-monitoring-guide.md # 代码监控指南
├── 📁 public/               # 静态资源
├── 📁 scripts/              # 构建脚本
│   ├── naming-rules.ts      # 命名规范检查
│   ├── check-env.cts        # 环境变量检查
│   ├── cc-admin-monitor.sh  # 本地代码监控脚本
│   └── advanced-search.sh   # 高级搜索脚本
├── 📁 src/                  # 源代码目录
│   ├── 📁 api/              # API接口管理
│   │   ├── index.ts         # API统一导出
│   │   └── modules/         # 具体API模块
│   ├── 📁 assets/           # 静态资源
│   │   ├── icons/           # 图标资源
│   │   └── styles/          # 全局样式
│   ├── 📁 common/           # 公共模块
│   │   ├── index.ts         # 公共模块统一导出
│   │   └── modules/         # 具体公共功能
│   │       ├── constants.ts # 常量定义
│   │       ├── function.ts  # 工具函数
│   │       ├── helpers.ts   # 辅助函数
│   │       └── route.ts     # 路由工具
│   ├── 📁 components/       # 公共组件
│   │   ├── common/          # 通用组件
│   │   └── layout/          # 布局组件
│   ├── 📁 hooks/            # 组合式函数
│   │   ├── index.ts         # Hooks统一导出
│   │   └── modules/         # 具体Hook模块
│   ├── 📁 layouts/          # 布局模板
│   │   ├── components/      # 布局组件
│   │   └── index.vue        # 主布局入口
│   ├── 📁 locales/          # 国际化
│   │   ├── index.ts         # 国际化配置
│   │   ├── lang/            # 语言包
│   │   ├── modules/         # 分模块翻译
│   │   └── types.ts         # 国际化类型
│   ├── 📁 router/           # 路由管理
│   │   ├── index.ts         # 路由统一导出
│   │   ├── modules/         # 路由模块
│   │   └── utils/           # 路由工具
│   ├── 📁 stores/           # 状态管理
│   │   ├── index.ts         # Store统一导出
│   │   └── modules/         # 具体Store模块
│   │       ├── app.ts       # 应用状态
│   │       ├── user.ts      # 用户状态
│   │       ├── color.ts     # 主题颜色
│   │       ├── size.ts      # 尺寸配置
│   │       ├── layout.ts    # 布局状态
│   │       ├── locale.ts    # 语言状态
│   │       ├── permission.ts # 权限状态
│   │       └── postcss.ts   # PostCSS适配
│   ├── 📁 Types/            # 类型定义
│   │   ├── env.d.ts         # 环境变量类型
│   │   ├── global.d.ts      # 全局类型
│   │   └── router.d.ts      # 路由类型
│   ├── 📁 utils/            # 工具函数
│   │   ├── http/            # HTTP请求工具
│   │   ├── deviceInfo.ts    # 设备信息
│   │   ├── env.ts           # 环境工具
│   │   └── moduleLoader.ts  # 模块加载器
│   ├── 📁 views/            # 页面组件
│   │   ├── dashboard/       # 仪表盘
│   │   ├── example/         # 示例页面
│   │   ├── login/           # 登录页面
│   │   └── user/            # 用户管理
│   ├── App.vue              # 根组件
│   └── main.ts              # 应用入口
├── 📄 eslint.config.ts      # ESLint配置
├── 📄 package.json          # 项目配置
├── 📄 tsconfig.json         # TypeScript配置
├── 📄 uno.config.ts         # UnoCSS配置
├── 📄 vite.config.ts        # Vite配置
└── 📄 README.md             # 项目说明
```

---

## 🔍 代码监控

CC-Admin 框架配备了完整的代码监控系统，用于保护知识产权和检测抄袭行为。

### 监控功能

- **🛡️ 版权保护**: 基于独特标识符的精确检测
- **🏗️ 结构分析**: 检测文件组织和模块结构抄袭
- **⚡ 技术栈识别**: 识别相似的技术栈组合
- **📊 自动监控**: GitHub Actions 定时扫描
- **🔔 即时通知**: 多渠道通知（邮件、企业微信、钉钉）

### 使用方法

```bash
# 本地监控
export GITHUB_TOKEN="your_github_token"
pnpm monitor

# 快速搜索
pnpm monitor:quick
```

### 监控配置

1. **GitHub Actions**: 每周自动执行
2. **本地脚本**: 支持手动执行和详细分析
3. **通知系统**: 发现问题时自动发送警报

详细配置请查看 [代码监控指南](./docs/code-monitoring-guide.md)

---

## 📚 开发指南

### 项目约定

#### 1. 模块组织规范

所有功能模块遵循 **`index.ts + modules/`** 统一结构：

```typescript
// src/stores/index.ts - 统一导出入口
export * from './modules/app'
export * from './modules/user'
// ... 其他模块

// src/stores/modules/user.ts - 具体实现
export const useUserStore = defineStore('user', {
  // store 实现
})
```

#### 2. 自动导入机制

框架使用 `autoImportModulesSync` 实现模块自动装载：

```typescript
// 自动扫描 modules/ 目录下的所有模块
const modules = import.meta.glob('./modules/**/*.ts', { eager: true })
const importedModules = autoImportModulesSync(modules)
```

#### 3. 命名规范

- **文件命名**: kebab-case (如 `user-service.ts`)
- **组件命名**: PascalCase (如 `UserCard.vue`)
- **函数变量**: camelCase (如 `getUserInfo`)
- **常量**: SCREAMING_SNAKE_CASE (如 `API_BASE_URL`)
- **类型接口**: PascalCase (如 `UserInfo`)

#### 4. 实时命名规范检查

项目提供实时监听功能，自动检查文件命名规范：

```bash
# 启动实时监听
pnpm naming-watch

# 详细模式（显示更多信息）
pnpm naming-watch --verbose
```

监听器会自动检查：

- 新建文件的命名规范
- 修改文件的内容规范
- 提供实时的错误提示和建议

### 开发工作流

#### 1. 功能开发

```bash
# 1. 创建功能分支
git checkout -b feat/new-feature

# 2. 开发功能（自动启动命名规范监听）
pnpm dev

# 3. 代码检查
pnpm check

# 4. 规范提交
pnpm commit

# 5. 推送分支
git push origin feat/new-feature
```

#### 2. 添加新页面

```bash
# 1. 在 src/views/ 创建页面目录
mkdir src/views/new-page

# 2. 创建页面文件
touch src/views/new-page/index.vue

# 3. 添加路由配置
# 在 src/router/modules/ 添加路由文件

# 4. 更新导航菜单
# 在对应的布局组件中添加菜单项
```

#### 3. 添加新的 Store

```typescript
// src/stores/modules/new-store.ts
export const useNewStore = defineStore('new-store', {
  state: () => ({
    // 状态定义
  }),
  getters: {
    // 计算属性
  },
  actions: {
    // 方法定义
  },
})

// src/stores/index.ts - 添加导出
export * from './modules/new-store'
```

#### 4. 添加API模块

```typescript
// src/api/modules/new-api.ts
export const newAPI = {
  // API 方法定义
}

// src/api/index.ts - 添加导出
export * from './modules/new-api'
```

### 样式开发

#### 1. UnoCSS 使用

```vue
<template>
  <!-- 使用原子化类名 -->
  <div class="flex items-center justify-between p-4 bg-white rounded-lg shadow-sm">
    <h1 class="text-xl font-bold text-gray-800">标题</h1>
    <button class="btn btn-primary">按钮</button>
  </div>
</template>
```

#### 2. 主题系统

```typescript
// 使用主题颜色
const colorStore = useColorStore()

// 切换主题
colorStore.toggleTheme()

// 设置主题色
colorStore.setPrimaryColor('#1890ff')
```

#### 3. 响应式适配

```typescript
// 使用响应式工具
const sizeStore = useSizeStore()

// 获取当前尺寸预设
const currentSize = sizeStore.currentSize

// 切换尺寸预设
sizeStore.setSizePreset('comfortable')
```

---

## 🔧 配置说明

### 环境变量

项目使用三个环境文件：

- `.env` - 基础环境变量
- `.env.development` - 开发环境变量
- `.env.production` - 生产环境变量

详细说明请查看 [环境变量文档](./docs/environment-variables.md)

### 构建配置

Vite 配置文件 `vite.config.ts` 包含：

- 路径别名配置
- 插件配置
- 构建优化
- 开发服务器配置

### 代码规范

ESLint 配置 `eslint.config.ts` 包含：

- Vue 3 规则
- TypeScript 规则
- 自定义命名规范
- 代码质量规则

---

## 🚀 部署

### 构建生产版本

```bash
# 构建生产版本
pnpm build

# 预览构建结果
pnpm preview

# 构建分析
pnpm build:analyze
```

### 部署到服务器

```bash
# 1. 构建项目
pnpm build

# 2. 将 dist/ 目录内容上传到服务器
scp -r dist/* user@server:/path/to/webroot/

# 3. 配置 Nginx（示例）
# server {
#   listen 80;
#   server_name your-domain.com;
#   root /path/to/webroot;
#   index index.html;
#   location / {
#     try_files $uri $uri/ /index.html;
#   }
# }
```

---

## 📖 相关文档

### 核心系统指南

- [🏗️ 项目架构设计](./docs/architecture-guide.md) - 整体架构设计和设计原则
- [💾 状态管理指南](./docs/pinia-guide.md) - Pinia 状态管理完整指南
- [🛣️ 路由配置指南](./docs/router-guide.md) - Vue Router 路由系统指南
- [🌐 API 管理指南](./docs/api-guide.md) - Alova 网络请求管理
- [🎨 UnoCSS 使用指南](./docs/unocss-guide.md) - 原子化 CSS 使用指南
- [🧩 组件开发指南](./docs/component-guide.md) - Vue 组件开发规范

### 安全与质量

- [🔒 安全管理指南](./docs/security-guide.md) - 身份认证和权限控制安全体系
- [⚡ 性能优化指南](./docs/performance-guide.md) - 构建优化和运行时性能优化
- [🧪 测试指南](./docs/testing-guide.md) - 单元测试、组件测试、E2E测试策略
- [🔍 代码监控指南](./docs/code-monitoring-guide.md) - 代码监控和保护系统

### 部署与运维

- [🚀 部署指南](./docs/deployment-guide.md) - 多环境部署和CI/CD流程
- [🛠️ 故障排除指南](./docs/troubleshooting-guide.md) - 常见问题诊断和解决方案

### 工程化配置

- [🔧 构建配置指南](./docs/build-guide.md) - Vite 构建系统配置
- [⚙️ 开发工具链指南](./docs/toolchain-guide.md) - ESLint、Prettier、TypeScript工具链
- [🌍 环境变量配置](./docs/environment-variables.md) - 环境变量管理指南
- [🌐 国际化配置](./docs/locale.md) - Vue I18n 国际化配置详解
- [📱 响应式适配](./docs/rem-adapter.md) - rem 适配系统详解

### 开发工具

- [🎯 Cursor 配置说明](./.cursor/README.md) - AI 编程助手配置

---

## 🤝 贡献

我们欢迎各种形式的贡献！请阅读我们的贡献指南：

1. Fork 本仓库
2. 创建特性分支 (`git checkout -b feat/amazing-feature`)
3. 提交更改 (`pnpm commit`)
4. 推送到分支 (`git push origin feat/amazing-feature`)
5. 创建 Pull Request

### 提交规范

使用 [Conventional Commits](https://conventionalcommits.org/) 规范：

```
feat: 添加新功能
fix: 修复bug
docs: 更新文档
style: 代码样式修改
refactor: 代码重构
test: 添加测试
chore: 构建过程或辅助工具的变动
```

---

## 📄 许可证与版权

### 版权声明

本项目由 **chichuang** 开发并维护，采用 [自定义商业限制许可证](./LICENSE)。

### 使用条款

**允许的行为：**

- ✅ 个人学习、研究使用
- ✅ 开源项目中的非商业使用
- ✅ Fork 和贡献代码
- ✅ 在保留版权声明的前提下修改和分发

**禁止的行为：**

- ❌ **商业用途**：未经授权不得用于商业项目或收费服务
- ❌ **删除署名**：不得删除或修改原作者版权信息
- ❌ **冒充原创**：不得声称是原创作品或删除原作者署名
- ❌ **恶意抄袭**：不得直接复制项目结构、UI设计用于商业产品

### 商业授权

如需商业使用或合作，请联系：

- **作者**: chichuang
- **项目**: CC-Admin 企业级后台管理框架
- **联系方式**: [请通过 GitHub Issues 联系](https://github.com/你的用户名/cc-admin/issues)

### 版权保护

本项目已采取以下保护措施：

- 📄 完整的自定义商业限制许可证
- 🔍 源码文件头部版权注释
- 📝 README 详细使用条款
- 🛡️ GitHub Actions 自动检查
- 🔒 自动化版权保护工具
- �� 代码监控和保护系统

---

## 🔧 环境配置

### GitHub Token 配置

代码监控系统需要 GitHub Token 来访问 API。请按以下步骤配置：

#### 1. 获取 GitHub Token

1. 登录 GitHub → Settings → Developer settings → Personal access tokens → Tokens (classic)
2. 点击 "Generate new token (classic)"
3. 设置描述：`CC-Admin 代码监控系统`
4. 选择权限：`repo`, `read:org`, `read:user`, `read:email`
5. 生成并复制 Token

#### 2. 配置 Token

```bash
# 方法1: 环境变量
export GITHUB_TOKEN="your_token_here"

# 方法2: .env 文件 (推荐)
echo "GITHUB_TOKEN=your_token_here" > .env

# 方法3: 直接传递
GITHUB_TOKEN="your_token_here" pnpm monitor
```

#### 3. 测试配置

```bash
# 测试 Token 有效性
pnpm token:test

# 运行完整监控
pnpm monitor
```

详细配置说明请查看：[GitHub Token 配置指南](docs/github-token-guide.md)

---

## 🙏 致谢

感谢以下优秀的开源项目：

- [Vue.js](https://vuejs.org/) - 渐进式JavaScript框架
- [Vite](https://vitejs.dev/) - 下一代前端构建工具
- [UnoCSS](https://unocss.dev/) - 即时原子化CSS引擎
- [Pinia](https://pinia.vuejs.org/) - Vue状态管理库
- [TypeScript](https://www.typescriptlang.org/) - JavaScript超集

---

<p align="center">
  Made with ❤️ by <strong>chichuang</strong>
</p>
