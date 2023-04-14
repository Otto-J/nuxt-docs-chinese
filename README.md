# nuxt-docs-chinese

- raw 分支，实时 nuxt/nuxt 的 docs 文件夹
- docs 分支，翻译文件夹

这个 GitHub Actions 工作流程包括以下几个步骤：

在计划时间或手动触发时运行。
检出仓库的 raw 分支。
设置 Node.js 环境。
下载 nuxt/nuxt 项目的 docs 文件夹并强制推送到 raw 分支。
尝试将 raw 分支合并到 docs 分支。如果合并成功，直接推送；否则，自动创建一个包含合并冲突的 PR，以便手动解决冲突。
请注意，您需要在仓库设置中创建一个名为 GITHUB_TOKEN 的密钥，以便 GitHub Actions 能够访问您的仓库。这个文件应该放在您的代码仓库的 .github/workflows 文件夹中。
