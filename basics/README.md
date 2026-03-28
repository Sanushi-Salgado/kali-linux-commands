# ⚡💻 Kali Linux Commands 🐉⚡

---

## 🧠⚙️ Basic Operators & Command Chaining

```bash
;       														# 🔗 Run multiple commands in one line
&&      														# ✅ Run next command only if previous succeeds
|       														# 🔄➡️ Pipe output from one command into another ex: ls | pwd  
```

---

## 📁🗂️ File & Directory Operations

```bash
mkdir															# 📂 Create new directory
cd                             									# 📁➡️ Change directory
cd ..                          									# ⬆️ Move one directory up
cd ../..                       									# ⏫ Move two directories up
cd ~                           									# 🏠 Go to home directory 
mkdir results && cd results    									# 📂⚡ Create + enter directory
ls                             									# 👀 List directory contents
ls -l        													# 📄🔍 Detailed list: permissions, owner, size, timestamp
ls -la       													# 👀📂 Include hidden files (dotfiles) in detailed view
ls --help    													# ❓ Quick help / usage information for ls command
man ls       				 									# ❓ Open full manual for the ls command
pwd                            									# 📍 Show current path / working directory
```

---

## 🌐📡 Networking 

```bash
ifconfig                       									# 📡 Show network interfaces & local IP addresses (legacy)
curl ifconfig.me              									# 🌍 Get your public (external) IP address
ip a                            								# 🌐 Show IP addresses & network interfaces (modern)
ping <IP address>             									# 📶 Test connectivity to a specific IP address
ping <domain>            										# 🌍 Test connectivity to a domain name
ping -c 3 <domain>            									# 📊 Send only 3 ping packets
nslookup <domain or subdomain>            					    # 🔍 Get DNS information for a domain
netstat                       									# 🔌 Show active network connections
netstat -tulnp                									# 📊 Show listening ports & services with details
ss -tulnp                      									# ⚡ Faster modern alternative to netstat
traceroute <domain>          									# 🛰️ Trace the path packets take to destination
```

---

## 👤🕵️ User Info

```bash
whoami                         									# 🙋 Current user
id                             									# 🧾 User details (UID, groups)
```

---

## 💻🕵️ System Info

```bash
uname -a             											# 🖥️ Kernel + system info
cat /etc/os-release  											# 🐧 OS version & distribution details
```

---

## 🧹🧼 Terminal Cleanup

```bash
clear                          									# 🧽 Clear terminal
history -c && history -w && hash -r								# 🧨 Full cleanup (history reset)
```

---

## 🔐🛡️ Privilege Control

```bash
sudo command                   									# 👑 Execute as root / superuser
su                             									# 🔄👤 Switch user
```

---

## 📦📡 Package Management (APT)

### 🔄 Update & Upgrade

```bash
sudo apt update 												# 📡 Update system
sudo apt upgrade or sudo apt upgrade -y 						# ⬆️ Upgrade all packages 
sudo apt update && sudo apt upgrade -y  						# ⚡ Run above both commands together
sudo apt install -f 											# 🛠️ Fix broken dependencies & complete pending installations

```

---

### 🐉 Full Kali Rolling Upgrade
> Fully upgrade Kali Linux VM to the latest rolling release️.
> ⚠ Backup recommended before full upgrade.


```bash
sudo cp /etc/apt/sources.list /etc/apt/sources.list.bak && \
sudo sed -i 's|.*|deb http://http.kali.org/kali kali-rolling main non-free contrib|' /etc/apt/sources.list && \
sudo apt update && \
sudo apt -y full-upgrade && \
sudo apt -y autoremove && \
sudo apt -y autoclean && \
sudo reboot
```

---

### 🧽 Cleanup

```bash
sudo apt autoremove -y        									# 🧹 Remove unused packages
sudo apt clean                									# 🗑️ Clear local package cache
sudo apt autoclean            									# ♻️ Remove outdated packages
```

---

## ⚡🛠️ System Maintenance

```bash
# 🧹 Clear traces + clean system (clear bash history, reset command cache, clean apt cache)
history -c && history -w && hash -r && sudo apt clean && sudo apt autoclean 
```

---

## 💤🚫 Prevent System Sleep
> Keep system awake without sleeping

```bash
sudo systemctl mask sleep.target suspend.target hibernate.target
xset s off -dpms
```

---

## 🔁🔌 System Reboot

```bash
sudo reboot														# 🔄 Restart system
```

---

## 📝📂 File Display

```bash
cat path/to/file or filename                                    # 📜 Display the content of the file in the terminal
cat path/to/file or filename | less                             # 🖼️ Display the content of the file one page at a time (for large files)
cat path/to/file or filename | grep "search_term"               # 🔍 Search for a specific term within the file's content
cat path/to/file or filename > newfile                          # 📥 Copy the content of a file into a new file
cat path/to/file or filename >> existingfile                    # 📤 Append the content of a file to an existing file
cat -n path/to/file or filename                                 # 🔢 Display the content with line numbers
cat -b path/to/file or filename                                 # 🧮 Display the content with line numbers for non-blank lines
```

---

## 📝✏️ File Editing

```bash
nano path/to/file or filename 									# ✍️ Edit file via nano
sudo nano path/to/file or filename								# 🔐✍️ Edit file via nano as root
```

---

## ⌨️⚡ Keyboard Shortcuts

```bash
Ctrl + Alt + T 													# 🖥️ Open new terminal 					
Shift + Insert 													# 📋 Paste          					
Ctrl + A      													# 🔘 Select all     					
```

---

## ⚠️ Disclaimer
> This repository is for **educational purposes only**.  
> Misuse may result in system damage, data loss, or legal consequences.  
> Always obtain proper authorization & practice **ethical usage**.