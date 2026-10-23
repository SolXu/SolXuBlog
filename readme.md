# Solxu Blog

计划采用 Astro + Vue + TypeScript。当前仓库为 Astro 基础脚手架，已启用 TypeScript 严格配置，尚未添加 Vue 集成。

项目已迁移到仓库根目录，以下命令均在根目录执行。

## 环境要求

- Node.js >= 22.23.4
- npm

根据锁文件安装依赖：

```sh
npm ci
```

## 本地开发

以后台模式启动开发服务器，默认地址为 `http://localhost:4321`：

```sh
npm run dev -- --background
```

查看状态、读取日志和停止后台服务器：

```sh
npm run astro -- dev status
npm run astro -- dev logs
npm run astro -- dev stop
```

## 构建与预览

```sh
npm run build
npm run preview
```

构建产物位于 `dist/`，预览命令用于查看已生成的构建产物。

## 项目结构

```text
public/             静态资源
src/assets/         页面使用的资源
src/components/     Astro 组件
src/layouts/        页面布局
src/pages/          页面与路由
astro.config.mjs    Astro 配置
tsconfig.json       TypeScript 配置
```

开发约定见 [AGENTS.md](./AGENTS.md)，框架文档见 [Astro 官方文档](https://docs.astro.build)。
