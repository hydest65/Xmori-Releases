# Xmori Windows Preview

This repository distributes Xmori Windows x64 preview programs and signed update manifests. The Xmori source repository is private. User workspaces, documents, model credentials and signing private keys are never distributed here.

Xmori is an independent local Windows desktop agent with its own Native runtime. Updating it does not require Codex or a GitHub account.

## First installation

Download the ZIP from an explicitly confirmed preview Release, extract all four components together into a writable application folder, and open `xusen-desktop.exe`. Select a separate data folder for your workspace. Keep the Desktop, Control, Office runtime and Image runtime together.

Preview.116 is the corrected update bootstrap for Windows PowerShell5.1. Earlier previews need this one-time manual installation to obtain the current updater and publisher trust. For the initial trust decision, confirm the download source and published SHA-256 through your trusted distributor. Subsequent versions are verified against the embedded update public key.

## Later updates

Open Settings → General → Check for updates, review the release notes, download and verify, then choose Restart and install. Pending tasks and approvals must finish first. The updater retains paired program and workspace backups and confirms that the selected workspace and Native service are ready.

Preview updates use RSA-SHA256 signed manifests and SHA-256 package verification. Windows binaries do not yet have an Authenticode publisher certificate, so Windows may report an unknown publisher. This preview channel is separate from the requirements for a formally signed stable release.

On interrupted installation, reopen Xmori to recover the complete prior program set. Workspace backups are retained and are never automatically copied over newer user data. If a new window cannot finish startup, close it normally before retrying recovery; do not replace running program files.

The package includes third-party runtime license notices. Download assets are programs, not a source-code license grant.
