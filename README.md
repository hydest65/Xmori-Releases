# Xmori 旭森 · Windows 测试版

Xmori 是面向 Windows 的 AI 工作台，可以查资料、改代码、处理文档和表格，也可以生成图片。

**[下载 Windows x64 测试版 · Downloads & release notes](https://github.com/hydest65/Xmori-Releases/releases)**

- **首次试用**　完整解压便携包到可写的新文件夹，双击最外层的 **Xmori.exe**。项目、任务和对话保存在同级的「测试数据」中。[下载 preview.131 便携测试包](https://github.com/hydest65/Xmori-Releases/releases/download/testers-v0.2.0-preview.131/Xmori-Tester-0.2.0-preview.131-windows-x64.zip)
- **已有新版更新通道的用户**　在「设置 → 常规 → 检查更新」查看 .131 的说明，点击「下载更新」，完成后选择「重启并安装」。[常规更新包与版本说明](https://github.com/hydest65/Xmori-Releases/releases/tag/preview2-v0.2.0-preview.131)
- **.130 便携版提示更新组件未完成**　正常退出后解压新版便携包，把新版的 **program** 文件夹和 **Xmori.exe** 复制到原测试目录并替换，保留原有「测试数据」。
- 第一代客户端沿用原签名通道，切换到新通道时需要手动安装一次引导版。

## English

This repository distributes Xmori Windows x64 preview programs and signed update manifests. The Xmori source repository is private. User workspaces, documents, model credentials and signing private keys are never distributed here.

Xmori is an independent local Windows desktop agent with its own Native runtime. Updating it does not require Codex or a GitHub account.

## First installation

For a clean tester workspace, extract the portable ZIP to a writable folder and open the top-level **Xmori.exe**. Always reuse that entry to keep your own projects and conversations. [Portable tester release](https://github.com/hydest65/Xmori-Releases/releases/tag/testers-v0.2.0-preview.131)

On the current signed-update channel, open **Settings → General → Check for updates**, download the update, and choose **Restart and install**. First-generation clients require a manual bootstrap to switch signing channels. [Standard release](https://github.com/hydest65/Xmori-Releases/releases/tag/preview2-v0.2.0-preview.131)


## Later updates

The main sidebar shows a reminder when a newer version is available. Select it, or open Settings → General → Check for updates, review the release notes, download and verify, then choose Restart and install. Background checks read public version metadata only; downloading and installation always require your action. Pending tasks and approvals must finish first. The updater retains paired program and workspace backups and confirms that the selected workspace and Native service are ready.

Preview updates use RSA-SHA256 signed manifests and SHA-256 package verification. Windows binaries do not yet have an Authenticode publisher certificate, so Windows may report an unknown publisher. This preview channel is separate from the requirements for a formally signed stable release.

On interrupted installation, reopen Xmori to recover the complete prior program set. Workspace backups are retained and are never automatically copied over newer user data. If a new window cannot finish startup, close it normally before retrying recovery; do not replace running program files.

The package includes third-party runtime license notices. Download assets are programs, not a source-code license grant.
