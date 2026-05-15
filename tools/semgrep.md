# 💻 Semgrep Commands 🐉

---

## 🔄 Installation

```bash
pipx install semgrep										# 📦 Install Semgrep via pipx (isolated environment)
pipx upgrade semgrep										# 🔄 Upgrade Semgrep via pipx to the latest version
```

---

## ✅ Verification 

```bash
which semgrep   											# 📍 Show the path to the installed Semgrep executable
semgrep --version											# 🛠️ Show the installed Semgrep version
semgrep --help												# ❓ Display help information for Semgrep 
semgrep scan --help											# ❓ Display help information for Semgrep scan command
```

---
## 🛠️ Usage

```bash
sudo tee /recon/semgrep-rules/custom.yml > /dev/null <<'EOF'# 📄 Create custom Semgrep rules file via terminal
rules:
  - id: example-rule
    pattern: fetch($URL)
    message: Possible SSRF sink detected
    severity: WARNING
    languages: [javascript, typescript]
EOF

semgrep scan                                                # 🔍 Run Semgrep scan (run inside repo folder)

semgrep scan \												# 🔍 Run Semgrep scan with rule packs & custom ruleset
  --json \
  --config=p/security-audit \
  --config=p/secure-defaults \
  --config=p/r2c-security-audit \
  --config=p/owasp-top-ten \
  --config=p/cwe-top-25 \
  --config=p/secrets \
  --config=p/xss \
  --config=p/sql-injection \
  --config=p/command-injection \
  --config=p/comment \
  --config=p/flask \
  --config=p/java \
  --config=p/javascript \
  --config=p/typescript \
  --config=p/react \
  --config=p/ruby \
  --config=p/python \
  --config=p/php \
  --config=p/csharp \
  --config=p/insecure-transport \
  --config=p/docker \
  --config=p/kubernetes \
  --config=p/terraform \
  --config=p/ci \
  --config=p/docker-compose  \
  --config=p/dockerfile \
  --config=p/kubernetes \
  --config=p/nginx \
  --config=p/terraform \
  --config=/home/osboxes/Documents/semgrep_rules.yml \
  --no-git-ignore \
  --disable-version-check \
  --timeout=0 \
  .
```
