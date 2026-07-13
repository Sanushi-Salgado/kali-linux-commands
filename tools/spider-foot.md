# 💻 SpiderFoot Commands 🐉

---

## ✅ Verification 

```bash
spiderfoot --version     										 # 🛠️ Get the installed SpiderFoot version

which spiderfoot      											 # 📍 Get the path to the installed SpiderFoot executable

spiderfoot -h													 # ❓ Get help / usage information for SpiderFoot
```

---

## 🛠️ Usage

```bash
spiderfoot -M													 # 🧩 Get available modules

spiderfoot -s <domain>      									 # 🌐 Get information related to a domain via default enabled modules

spiderfoot -s <domain> -m <module>	               				 # 🌐 Get information related to a domain via a specific module

spiderfoot -s <domain> -u passive -o json -q > spiderfoot.json   # 🔇 Run passive scan for the given domain while surpressing background output & get results in JSON format

spiderfoot -s <domain> -u passive -o json > spiderfoot.json      # 🌐 Run passive scan for the given domain while displaying background output & get results in JSON format
```