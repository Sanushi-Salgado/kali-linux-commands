# 💻 DBeaver Commands 🐉

## ⚡ Prerequisites

```bash
1. Install dpkg package manager if not already installed.
sudo apt install dpkg   										

2. Download the Linux DEB file via the below link.
https://dbeaver.io/download/?start&os=linux&arch=x86_64&dist=deb

3. Navigate to the downloaded directory & check the version no of the downloaded file.
ls
```

---

## 🔄 Installation

```bash
sudo dpkg -i dbeaver-ce-<version no>-linux-x86_64.deb                  # 📦 Install DBeaver from .deb package
sudo apt --fix-broken install                                          # 🛠️ Fix broken dependencies (if any)
```

---

## ✅ Verification 

```bash
dbeaver                                                                # 🚀 Launch DBeaver
```
