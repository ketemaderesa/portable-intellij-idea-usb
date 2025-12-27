# portable-intellij-idea-usb
Portable IntelliJ IDEA setup on USB using Portapps or official ZIP, with settings and plugins stored locally.
# Portable IntelliJ IDEA on USB (Windows)

This repository provides **two reliable methods** to run **IntelliJ IDEA** in portable mode from a USB drive.

✅ No installation on host PC  
✅ Works on restricted systems  
✅ Plugins and settings stay on USB  

---

## 🔧 Requirements

- Windows OS
- USB drive (USB 3.0+ recommended)

---

## 🟢 Method 1: Portapps (Recommended – Easiest)

### ✔ Community Edition (Free)
https://portapps.io/app/intellij-idea-community-portable/

### ✔ Ultimate Edition (Paid)
https://portapps.io/app/intellij-idea-ultimate-portable/

---

### 📂 Steps (Portapps)

1. Download the portable `.exe`
2. Run it and select your USB drive:
3. Files are extracted directly to USB
4. Run IntelliJ using:
   
All settings, plugins, and caches remain on the USB.

---

## 🟡 Method 2: Official JetBrains ZIP (Manual Setup)

### 📥 Download

- https://www.jetbrains.com/idea/download/
- Choose **Windows → ZIP** (not `.exe`)

---

### 📂 Setup Portable Mode

1. Extract ZIP to USB:

2. Create data folders:

E:\IntelliJ\data
├── config
├── system
├── plugins


3. Open:
E:\IntelliJ\bin\idea.properties

4. Add or edit:
```properties
idea.config.path=../data/config
idea.system.path=../data/system
idea.plugins.path=../data/plugins
▶️ Run IntelliJ IDEA
E:\IntelliJ\bin\idea64.exe
All configurations and plugins are saved on the USB.
🔄 Updating IntelliJ IDEA

Download the newer ZIP version

Extract over the existing IntelliJ folder

Keep the data directory unchanged
⚠️ Notes

First startup may take longer on slower USB drives

Do not unplug USB while IntelliJ is running
This repository is documentation only.
IntelliJ IDEA is licensed by JetBrains.
