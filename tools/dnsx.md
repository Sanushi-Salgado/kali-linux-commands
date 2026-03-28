# 💻 DNSx Commands 🐉

---

## 🔄 Installation

```bash
go install github.com/projectdiscovery/dnsx/cmd/dnsx@latest		# 📦 Install DNSx (latest version) using Go
```

---

## ✅ Verification 

```bash
dnsx -version   												# 🛠️ Show the installed DNSx version
```

---

## 🛠️ Usage

```bash
echo <domain/subdomain> | dnsx -a -aaaa -cname -resp  			# 🌐 Enumerate DNS records for a domain/subdomain & show responses
```