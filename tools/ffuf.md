# 💻 Ffuf Commands 🐉

---

## ✅ Verification 

```bash
ffuf -V 	 													# 🛠️ Get the installed Ffuf version

which ffuff  													# 📍 Get the path to the installed Ffuf executable

ffuf -h 														# ❓ Get help / usage information for Ffuf
```

---

## 🛠️ Usage

```bash
ffuf                     										# 🚀 Launch Ffuf

ffuf \															# 🔍 Run Ffuf scan to find VHosts
  -c \
  -w <path of wordlist> \
  -u <scheme ex: http>://<domain or IP address> \
  -H "Host: FUZZ.<domain>" \
  -mc <status codes separated by comma> \
  -t <no of threads> \
  -rate <rate limit> \
  -timeout <timeout in seconds> \
  -maxtime <max runtime in seconds> \
  -k \
  -of <output format ex: json> \
  -o <path of output file>.json \
  -debug-log <path of log file>.log \
  -v 
```