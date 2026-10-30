# 💻 Bandit Commands 🐉

---

## 🔄 Installation

```bash
sudo apt install -y bandit                                        #  📦 Install Bandit via apt
```

---

## ✅ Verification 

```bash
which bandit 	                                                  # 📍 Show the path to the installed Bandit executable

bandit --version                                                  # 🛠️ Get the installed Bandit version

bandit --help                                                     # ❓ Get help / usage information for Bandit
```

---

## 🛠️ Usage

```bash
bandit -f json <path/to/python/file> > results.json		          # 🔎 Get security issues of a given Python file in JSON format
```