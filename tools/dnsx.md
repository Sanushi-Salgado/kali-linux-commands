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
echo <domain/subdomain> | dnsx -a -aaaa -cname -resp  			# 🌐 Enumerate & display DNS records for a domain/subdomain

echo <domain/subdomain> | dnsx -ns -json                        # 🔎 Display NS records for a domain/subdomain in JSON format

echo <subdomain> | dnsx -cname -json | jq                       # 🔎 Display CNAME records for a subdomain in JSON format

echo <IP> | dnsx -ptr -resp										# 🔎 Display PTR records for an IP 
```
