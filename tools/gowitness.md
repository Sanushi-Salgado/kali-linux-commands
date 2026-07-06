# 💻 Gowitness Commands 🐉

## ⚡ Prerequisites

```bash
1. Download the Linux binary
wget https://github.com/sensepost/gowitness/releases/download/<version>/gowitness-<version>-linux-amd64

2. Check what you actually downloaded
ls -lh gowitness-<version>-linux-amd64 

3. Check file type to verify if it’s a Linux executable
file gowitness-<version>-linux-amd64   
```

---

## 🔄 Installation

```bash
chmod +x gowitness-<version>-linux-amd64 					# 📦 Make it executable 

sudo mv gowitness-<version>-linux-amd64 /<path>  			# ➡️📁 Move it into PATH
```

---

## ✅ Verification 

```bash
gowitness version											# 🛠️ Show the installed gowitness version

gowitness --help 											# ❓ Display help information for Gowitness

gowitness scan --help										# ❓ Display help information for Gowitness	scan option	

gowitness scan single --help								# ❓ Display help information for Gowitness single scan option
```

---

## 🛠️ Usage

```bash
gowitness scan single \										# 📸📁 Capture & save screenshots of a single specified URL to a given directory
  --url <url / domain url> \
  --write-screenshots \
  --screenshot-path /<path>
```