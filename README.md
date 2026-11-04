# Xmori 旭森 · Windows 测试版

Xmori 是面向 Windows 的 AI 工作台，可以查资料、改代码、处理文档和表格，也可以生成图片。

**[下载 Windows x64 测试版 · Downloads & release notes](https://github.com/hydest65/Xmori-Releases/releases)**

- **首次安装**时，在发布页展开 **Assets**，下载名称以 `-windows-x64.zip` 结尾的程序包。核对发布方提供的 SHA-256，完整解压后打开 `xusen-desktop.exe`，为工作区选择单独的数据目录。
- **更新现有版本**时，可在 preview.118 或更高版本的「设置 → 常规 → 检查更新」中查看说明，下载并校验后选择「重启并安装」。preview.117 及更早版本请先从可信入口安装 [preview.118 引导版](https://github.com/hydest65/Xmori-Releases/releases/tag/v0.2.0-preview.118)。

## English

This repository distributes Xmori Windows x64 preview programs and signed update manifests. The Xmori source repository is private. User workspaces, documents, model credentials and signing private keys are never distributed here.

Xmori is an independent local Windows desktop agent with its own Native runtime. Updating it does not require Codex or a GitHub account.

## First installation

Download the ZIP from an explicitly confirmed preview Release, extract all four components together into a writable application folder, and open `xusen-desktop.exe`. Select a separate data folder for your workspace. Keep the Desktop, Control, Office runtime and Image runtime together.

Preview.118 is the corrected update bootstrap for Windows PowerShell5.1. Earlier previews need this one-time manual installation to obtain the current updater and publisher trust. For the initial trust decision, confirm the download source and published SHA-256 through your trusted distributor. Subsequent versions are verified against the embedded update public key.

## Later updates

The main sidebar shows a reminder when a newer version is available. Select it, or open Settings → General → Check for updates, review the release notes, download and verify, then choose Restart and install. Background checks read public version metadata only; downloading and installation always require your action. Pending tasks and approvals must finish first. The updater retains paired program and workspace backups and confirms that the selected workspace and Native service are ready.

Preview updates use RSA-SHA256 signed manifests and SHA-256 package verification. Windows binaries do not yet have an Authenticode publisher certificate, so Windows may report an unknown publisher. This preview channel is separate from the requirements for a formally signed stable release.

On interrupted installation, reopen Xmori to recover the complete prior program set. Workspace backups are retained and are never automatically copied over newer user data. If a new window cannot finish startup, close it normally before retrying recovery; do not replace running program files.

The package includes third-party runtime license notices. Download assets are programs, not a source-code license grant.
