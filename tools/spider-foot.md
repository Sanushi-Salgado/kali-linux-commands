# 💻 SpiderFoot Commands 🐉

---

## ✅ Verification 

```bash
spiderfoot --version     										 # 🛠️ Show the installed SpiderFoot version

which spiderfoot      											 # 📍 Show the path to the installed SpiderFoot executable

spiderfoot -h													 # ❓ Display help information for SpiderFoot
```

---

## 🛠️ Usage

```bash
spiderfoot -M													 # 🧩 View available modules

spiderfoot -s <domain>      									 # 🌐 View information related to a domain

spiderfoot -s <domain> -u passive -o json -q > spiderfoot.json   # 🔇 Run passive scan for the given domain while surpressing background output & get results in JSON format

spiderfoot -s <domain> -u passive -o json > spiderfoot.json      # 🌐 Run passive scan for the given domain while displaying background output & get results in JSON format
```