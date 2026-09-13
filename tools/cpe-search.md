# 💻 CPE Search Commands 🐉

## ⚡ Prerequisites

```bash
Install inside a virtual environment.

1. Create a virtual environment.
python3 -m venv ~/.venvs/cpe-search 

2. Activate the virtual environment.
source ~/.venvs/cpe-search/bin/activate

3. Upgrade pip.
pip install --upgrade pip
```


```
Install globally (system-wide) via pipx.
	
sudo apt update
sudo apt install -y pipx
pipx ensurepath
```

---

## 🔄 Installation

```bash
pip install cpe_search                                           #  📦 Install cpe_search via pip (isolated environment)

pipx install cpe_search                                          #  📦 Install cpe_search via pipx (globally)
```

---

## ✅ Verification 

```bash
cpe_search -V                                                    # 🛠️ Get the installed cpe_search version

cpe_search -h                                                    # ❓ Get help / usage information for cpe_search
```

---

## 🛠️ Usage

```bash
cpe_search -d                                                   # 📦 Download the prebuilt local database

cpe_search -q "Apache 2.4.39"                                   # 🔎 Get CPE resolution for the given technology & version
```
