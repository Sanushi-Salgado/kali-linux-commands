# 💻 Subwiz Commands 🐉

---

## 🔄 Installation

```bash
1. Create a virtual environment.
python3 -m venv subwiz-env                                               

2. Activate the virtual environment. 
source subwiz-env/bin/activate                
					
3. Install Subwiz via Pip.
pip install subwiz

4. Deactivate the virtual environment.   
deactivate

5. Open Bash configuration file.
nano ~/.bashrc

6. Add executables to the PATH (add one of the below commands to the file).
Use this: if no conflicts with other installed tools
export PATH="$PATH:$HOME/subwiz-env/bin" 

Use this: if conflicting with other installed tools
export PATH="/usr/local/bin:$HOME/go/bin:$PATH"

7. Save the file. Exit.

8. Reload Bash configuration.
source ~/.bashrc
```

---

## ✅ Verification 

```bash
subwiz -h																		# ❓ Get help / usage information for Subwiz
```