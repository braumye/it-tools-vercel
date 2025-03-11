# Vercel IT Tools

[![中文](https://img.shields.io/badge/中文-README.md-blue)](README.md)

This is a workflow repository that automatically deploys the [IT Tools](https://github.com/CorentinTh/it-tools) project to Vercel. The workflow runs automatically at 10:00 AM (UTC+8) daily and also supports manual deployment triggers.

## Features

- 🕙 Daily automatic deployment
- 🚀 Manual deployment support
- 🔄 Auto-sync with source repository
- ⚡ Vercel deployment integration

## Getting Started

1. Fork this repository
2. Create a new project in Vercel
3. Add the following secrets in your GitHub repository under Settings -> Secrets and variables -> Actions:
   - `VERCEL_TOKEN`: Vercel API token
   - `VERCEL_ORG_ID`: Vercel Organization ID
   - `VERCEL_PROJECT_ID`: Vercel Project ID

### Obtaining Vercel Configuration

1. VERCEL_TOKEN:
   - Visit [Vercel Settings](https://vercel.com/account/tokens)
   - Create a new token

2. VERCEL_ORG_ID and VERCEL_PROJECT_ID:
   - Run `vercel link` in your local project
   - Check the `.vercel/project.json` file for these values

## Manual Deployment

1. Go to the Actions tab in your repository
2. Select the "Deploy to Vercel" workflow
3. Click "Run workflow"

## License

MIT License

## Acknowledgments

- [IT Tools](https://github.com/CorentinTh/it-tools) - Original project
- [Vercel](https://vercel.com) - Deployment platform