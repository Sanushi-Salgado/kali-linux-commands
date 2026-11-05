# 💻 Cut-CDN Commands 🐉


## 🔄 Installation

```bash
go install github.com/ImAyrix/cut-cdn@latest		    		# 📦 Install Cut-CDN (latest version) via Go 

export PATH="$(go env GOPATH)/bin:$PATH" 			    		# ➡️📁 Add Go's binary directory to your PATH
```

---

## ✅ Verification 

```bash
which cut-cdn													# 📍 Get the path to the installed Cut-CDN executable

cut-cdn -v or cut-cdn --version	 								# 🛠️ Get the installed Cut-CDN version

cut-cdn -h or cut-cdn --help									# ❓ Get help / usage information for Cut-CDN
```

---

## 🛠️ Usage

```bash
cut-cdn -i <IP address>											# 🌐 Get information related to an IP address
```

---

## 🗑️ Uninstallation

```bash
sudo rm -f "$(which cut-cdn)"						   			# 🗑️ Uninstall Cut-CDN binary
```
