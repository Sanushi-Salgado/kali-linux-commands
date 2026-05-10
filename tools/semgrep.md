# 💻 Semgrep Commands 🐉

---

## 🔄 Installation

```bash
pipx install semgrep											# 📦 Install Semgrep using pipx (isolated environment)
```

---

## ✅ Verification 

```bash
which semgrep   												# 📍 Show the path to the installed Semgrep executable
```

---
## 🛠️ Usage

```bash
sudo tee /recon/semgrep-rules/custom.yml > /dev/null <<'EOF'    # 📄 Create a custom Semgrep rules file via terminal
rules:
  - id: example-rule
    pattern: fetch($URL)
    message: Possible SSRF sink detected
    severity: WARNING
    languages: [javascript, typescript]
EOF

semgrep scan                                                    # 🔍 Run a Semgrep scan (execute inside repo folder)
```
