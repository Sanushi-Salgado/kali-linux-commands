# 💻 Retire.js Commands 🐉

## ⚡ Prerequisites

```bash
1. Check if Node.js is installed
node -v

2. Check if NPM is installed
npm -v
```

---

## 🔄 Installation

```bash
sudo npm install -g retire                          # 📦 Install Retire.js via NPM

sudo npm install -g retire --verbose                # 📦 Install Retire.js via NPM with verbose logging
```

---

## ✅ Verification 

```bash
which retire                                        # 📍 Show the path to the installed Retire.js executable

retire --version                                    # 🛠️ Show the installed Retire.js version

retire -h                                           # ❓ Display help information for Retire.js
```

---

## 🛠️ Usage

```bash
retire --path <folder path>                          # 🔍 Run Retire.js scan 

retire \											 # 🔍 Run Retire.js scan using a local Retire.js vulnerability DB & get results in JSON format
  --path <folder path> \
  --jsrepo ~/retire-cache/jsrepository-v5.json \
  --outputformat json
```