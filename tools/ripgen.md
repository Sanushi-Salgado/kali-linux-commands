# 💻 Ripgen Commands 🐉

---

## 🔄 Installation

```bash
1. Update Kali packages.
sudo apt update

2. Install build tools (needed if Rust has to compile native dependencies).
sudo apt install build-essential curl -y

3. Install Rust via rustup.
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh

4. Reload shell.
source ~/.cargo/env

5. Verify Rust.
rustc --version
cargo --version

6. Install Ripgen.
cargo install ripgen
```

---

## ✅ Verification 

```bash
which ripgen										 		# 📍 Get the path to the installed Ripgen executable

ripgen --help												# ❓ Get help / usage information for Ripgen
```