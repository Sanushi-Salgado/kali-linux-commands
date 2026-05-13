# 💻 Github-Subdomains Commands 🐉

## ⚡ Prerequisites

```bash
1. Create Github token
GitHub > Settings > Developer settings > Personal Access Tokens > Tokens (classic) > Generate new token (classic) > Copy the token

2. Set your token as an environment variable
nano ~/.bashrc                                                 # Open the .bashrc file to edit

export GITHUB_TOKEN=<your_token>                               # Add this to the bottom of the file, save & exit

source ~/.bashrc                                               # Reload the .bashrc file

echo $GITHUB_TOKEN                                             # Print the value of your environment variable
```

---

## 🔄 Installation

```bash
go install github.com/gwen001/github-subdomains@latest        # 📦 Install Github-Subdomains using Go 
```

---

## ✅ Verification 

```bash
which github-subdomains                                       # 📍 Show the path to the installed Github-Subdomains executable

github-subdomains -h                                          # ❓ Display help / usage information for Github-Subdomains
```

---

## 🛠️ Usage

```bash
github-subdomains -d <domain>                                 # 🔍 Find subdomains under the given domain
```