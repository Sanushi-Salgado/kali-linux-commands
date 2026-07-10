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
retire --version                                    # 🛠️ Get the installed Retire.js version

which retire                                        # 📍 Get the path to the installed Retire.js executable

retire -h                                           # ❓ Get help / usage information for Retire.js
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