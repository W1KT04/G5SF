# G5SF - Rockstar / GTA Network Access Manager
**Version:** 2.5  
**Author:** W1KT04  

---

## Overview
G5SF (Grand Theft Auto / Rockstar Network Access Manager) is a Python-based tool for Windows that allows you to easily control the network access of Rockstar-related executables, such as GTA5.exe, Rockstar Games Launcher, Social Club, and more.

It works by automatically adding or removing Windows Firewall rules for these applications, letting you block or unblock their internet access with a simple menu interface.

---

## Features
- Block internet access for GTA5, Rockstar Launcher, Social Club, etc.  
- Unblock all previously created rules.  
- Display existing Rockstar or GTA-related firewall rules.  
- Built-in configuration file editor (`config.json`).  
- Automatic detection and elevation to administrator mode.  
- Uses Windows `netsh advfirewall` commands.  
- Clean, colorized terminal interface.

---

## Configuration
All application paths are stored in `config.json`.  
You can edit them manually or use the built-in editor in the program.

**Default config example:**
```json
{
    "paths": {
        "GTA5": [
            "C:\\SteamLibrary\\steamapps\\common\\Grand Theft Auto V\\GTA5.exe"
            "C:\\SteamLibrary\\steamapps\\common\\Grand Theft Auto V\\GTA5.exe"
        ],
        "Rockstar Games Launcher": [
            "C:\\Program Files\\Rockstar Games\\Launcher\\Launcher.exe"
        ],
        "RockstarService": [
            "C:\\Program Files\\Rockstar Games\\Launcher\\RockstarService.exe"
        ],
        "SocialClub": [
            "C:\\Program Files\\Rockstar Games\\Social Club\\SocialClub.exe"
        ]
    }
}
