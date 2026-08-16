# 💻 Tor Commands 🐉

---

## 🛠️ Usage

```bash
sudo systemctl start tor                                      # 🚀 Start the Tor service now

sudo systemctl stop tor                                       # 🛑 Stop the Tor service now

sudo systemctl enable tor                                     # 🔄 Make Tor start automatically at boot

sudo systemctl enable --now tor                               # 🔄 Enable Tor at boot & start it immediately

systemctl status tor                                          # 📊 Check if Tor is running

ss -lntp | grep 9050                                          # 🔎 Check if Tor is listening on SOCKS port 9050
```
