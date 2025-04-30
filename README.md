# OPTIMIZER_DEVICES
This project for optimizer devices pc

## DOCUMENTATION

🔧 1. Junk File Cleaner
📂 Targets:
Temp folders

Recycle bin

Cache directories (browser or OS-specific)

✅ Libraries:
Python

os, shutil, tempfile – for directory and file operations

send2trash – moves files to recycle bin instead of permanently deleting

Node.js (JavaScript)

fs-extra – for filesystem manipulation

trash – similar to send2trash

os – to get temp directories

PowerShell (called via Python/Node) – to access Windows cleanup features

🧬 2. Duplicate File Finder
🔍 Strategy:
Hash files (MD5, SHA256)

Compare files with the same size and hash

✅ Libraries:
Python

hashlib – for hashing files

os, glob – for directory walking

JavaScript (Node.js)

crypto – for hashing

fast-glob, fs – for file walking

🚀 3. Startup App Scanner
✅ On Windows:
Check HKCU\Software\Microsoft\Windows\CurrentVersion\Run in Registry

Check Task Scheduler

Check Startup folder

✅ Libraries:
Python

winreg – access Windows registry

subprocess – run PowerShell to list startup apps

Node.js

Use node-windows to access registry

Run PowerShell scripts using child_process

🔥 Bonus: System Performance Monitoring
Python: psutil – CPU, RAM, disk usage, running processes

Node.js: systeminformation, os-utils

🧰 Suggested Stack
For best access to Windows system internals:

Use Python for backend (file and registry operations)

Use Electron.js or Tkinter/PyQt for a desktop UI

Bundle with PyInstaller or pkg (Node.js) into an .exe

🧪 Tools to Explore:
pywin32 – Windows API access

wmi (Python) – system and hardware info

Electron + Node.js – for desktop GUI with backend logic
