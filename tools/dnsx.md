# 💻 DNSx Commands 🐉

---

## 🔄 Installation

```bash
go install github.com/projectdiscovery/dnsx/cmd/dnsx@latest							# 📦 Install DNSx (latest version) using Go
```

---

## ✅ Verification 

```bash
dnsx -version   											 						# 🛠️ Get the installed DNSx version
```

---

## 🛠️ Usage

```bash
echo <domain / subdomain> | dnsx -ns -json				 							# 🌐 Get NS records for a domain / subdomain in JSON format

echo <subdomain> | dnsx -cname -json | jq											# 🌐 Get CNAME records for a subdomain in JSON format

echo <IP address> | dnsx -ptr -resp						 							# 🌐 Get PTR records for an IP address

echo <domain / subdomain> | dnsx -a -aaaa -cname -resp								# 🌐 Get A, AAAA & CNAME records for a domain / subdomain

dnsx -json -silent -a -aaaa -cname -ns -txt -l <(echo domain / subdomain)			# 🌐 Get A, AAAA, CNAME, NS & TXT records for a domain / subdomain in JSON format
```