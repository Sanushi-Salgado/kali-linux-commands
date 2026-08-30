# 💻 PostgreSQL Commands 🐉

---

## ✅ Verification 

```bash
psql -V														# 🛠️ Get the installed PostgreSQL version

which psql													# 📍 Get the path to the installed PostgreSQL executable

psql --help													# ❓ Get help / usage information for PostgreSQL
```

## 🛠️ Usage

```bash
pg_lsclusters												# 🛠️ Check PostgreSQL cluster status

sudo pg_ctlcluster <version> main start						# 🚀 Start the cluster (if it's down)

sudo pg_ctlcluster <version> main restart					# 🔄 Restart the cluster

sudo -u postgres psql -c "\du"								# 👥 List DB roles / users

sudo -u postgres psql -c "\l"								# 📦 List databases
```