# EthStorage V1 Trusted Setup Ceremony - Step-by-Step Guide

Participate in the **EthStorage V1 Trusted Setup Ceremony** running from **August 13–22, 2025 (UTC)**.  

This global event strengthens the cryptographic foundations of EthStorage by generating secure parameters through community participation.  

**Deadline:** All contributions must be submitted before **August 22, 2025 (UTC)**.

<img width="1500" height="840" alt="image" src="https://github.com/user-attachments/assets/6979e9f7-e800-42e9-b8bf-f82e196b8cf4" />

---

## 1. Prerequisites

- **Supported OS**: Linux or macOS; or Windows via WSL 2
- **GitHub Account**:
  - At least 1 month old
  - At least 1 public repository
  - Follow 5+ GitHub accounts, 1+ follower
  - Enable reading/writing of **GitHub Gists**
- **Internet**: Stable and fast connection
- **Node.js & npm**:
  - Node.js 18+ and npm 9.2.0+
  - Recommended: Install via nvm

```bash
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash
source ~/.bashrc
nvm install 18
nvm use 18
```

---

## 2. Prepare Workspace

```bash
mkdir ~/trusted-setup-tmp && cd ~/trusted-setup-tmp
```

---

## 3. Install Ceremony CLI

```bash
npm install -g @p0tion/phase2cli
```

---

## 4. Authenticate via GitHub

```bash
phase2cli auth
```

<img width="1146" height="474" alt="image" src="https://github.com/user-attachments/assets/f72b5b42-5cbf-40a2-a73f-a6574580ab2e" />

- Opens browser to GitHub device login
- Paste code, authorize **p0tion** app

<img width="1600" height="894" alt="image" src="https://github.com/user-attachments/assets/1f282a17-7982-4c7b-a49a-db6c5845b5f2" />

- Return to terminal after “Congratulations, you’re all set!”

---

## 5. Contribute to the Ceremony

```bash
phase2cli contribute -c ethstorage-v1-trusted-setup-ceremony
```

- Provide entropy (CLI generates or type your own)
- **Do not** reuse or save this entropy
- If interrupted, rerun the same command to resume

---

## 6. Optional: Share on Twitter/X

After completing your contribution, you may be prompted to share it.

- Tag **@EthStorage** and use the hashtag **#EthStorage**
- Example:  
  > I just contributed to the EthStorage V1 Trusted Setup Ceremony! 🚀  
- **Privacy note**: Skip if you prefer to remain anonymous

---

## 7. After Contribution: Clean Up

```bash
phase2cli clean
phase2cli logout
rm -rf ~/trusted-setup-tmp
```

---

## 8. Troubleshooting

| Issue | Solution |
|-------|----------|
| Timeout: “you were removed as the current contributor” | Wait for timeout to expire, retry |
| “Timeout not yet expired” | Wait full timeout period, ensure stable internet |

---

## Quick Summary

1. Use Linux/macOS or WSL 2 with Node.js 18+  
2. Ensure GitHub account meets requirements  
3. Create working directory  
4. `npm install -g @p0tion/phase2cli`  
5. `phase2cli auth` → authorize on GitHub  
6. `phase2cli contribute -c ethstorage-v1-trusted-setup-ceremony`  
7. Optional: Share your participation on Twitter/X  
8. Clean up: `phase2cli clean`, `phase2cli logout`, remove directory  
9. Retry if timeouts occur

---

Your participation helps secure EthStorage for everyone.  
**Deadline:** August 22, 2025 (UTC)
