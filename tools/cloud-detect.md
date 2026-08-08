# 💻 CloudDetect Commands 🐉

## ⚡ Prerequisites

```bash
1. Update available software packages.
sudo apt update

2. Install Go.
sudo apt install golang-go

3. Verify Go version.
go version
```

---

## 🔄 Installation

```bash
go install github.com/99designs/clouddetect/cli/clouddetect@latest 				#	📦 Install CloudDetect (latest version) via Go
```

---

## ✅ Verification 

```bash
which clouddetect                                                               # 📍 Get the path to the installed CloudDetect executable

clouddetect -h                                                                  # ❓ Get help / usage information for CloudDetect

clouddetect --help                                                              # ❓ Get help / usage information for CloudDetect
```

---

## 🛠️ Usage

```bash
clouddetect -ip=<IP address>                                                    # 🌐 Get information related to an IP address
```
