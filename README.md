# Vercel IT Tools

[![English](https://img.shields.io/badge/English-README.en.md-blue)](README.en.md)

这是一个自动部署 [IT Tools](https://github.com/CorentinTh/it-tools) 项目到 Vercel 的工作流仓库。该工作流会在每天北京时间 10:00 自动执行，同时也支持手动触发部署。

## 功能特性

- 🕙 每天自动部署最新版本
- 🚀 支持手动触发部署
- 🔄 自动同步原仓库更新
- ⚡ 使用 Vercel 进行部署

## 使用方法

1. Fork 这个仓库
2. 在 Vercel 中创建新项目
3. 在 GitHub 仓库的 Settings -> Secrets and variables -> Actions 中添加以下密钥：
   - `VERCEL_TOKEN`: Vercel API token
   - `VERCEL_ORG_ID`: Vercel 组织 ID
   - `VERCEL_PROJECT_ID`: Vercel 项目 ID

### 获取 Vercel 配置

1. VERCEL_TOKEN:
   - 访问 [Vercel Settings](https://vercel.com/account/tokens)
   - 创建新的 Token

2. VERCEL_ORG_ID 和 VERCEL_PROJECT_ID:
   - 在本地项目中运行 `vercel link`
   - 查看 `.vercel/project.json` 文件获取

## 手动触发部署

1. 进入仓库的 Actions 页面
2. 选择 "Deploy to Vercel" 工作流
3. 点击 "Run workflow"

## 许可证

MIT License

## 致谢

- [IT Tools](https://github.com/CorentinTh/it-tools) - 原始项目
- [Vercel](https://vercel.com) - 部署平台