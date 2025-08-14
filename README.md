# Downloading to your offline machine later

1. From a connected machine, open your repo’s **Releases** page and download:

   * `anthropic-ai-claude-code-X.Y.Z.tgz`
   * (optionally) `anthropic-ai-claude-code-X.Y.Z.tgz.sha256`

2. Verify integrity (optional, on a connected or staging box):

```bash
sha256sum -c anthropic-ai-claude-code-X.Y.Z.tgz.sha256
```

3. Move the `.tgz` to the **offline** machine via USB.

4. **Install globally on the offline machine**:

```bash
# macOS/Linux:
npm install -g ./anthropic-ai-claude-code-X.Y.Z.tgz

# Windows (PowerShell):
npm install -g .\anthropic-ai-claude-code-X.Y.Z.tgz
```

> Note: The CLI installs offline fine, but **running it still requires access to Anthropic’s API** unless you have an on-prem/privately routed endpoint.


# Requirements:
- Node.js + npm
- gh (GitHub CLI) authenticated: gh auth login
- git remote "origin" pointing to your GitHub repo
