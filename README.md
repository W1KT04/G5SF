# G5SF — GTA 5 SERVICE OFF
**Version:** 2.2
**Author:** W1KT04  

---

## Overview
**G5SF** (Grand Theft Auto / gta 5 service off) is a Windows-based utility written in Python that provides fine-grained control over network access for Rockstar-related executables, such as **GTA5.exe**, **Rockstar Games Launcher**, **Social Club**, and supporting services.

By managing Windows Firewall rules automatically, G5SF enables users to block or restore network connectivity for these applications through a clean, interactive terminal interface — ideal for offline play, mod testing, or privacy control.

---

## Key Features
- **Network Control:** Block or unblock GTA5, Rockstar Launcher, Social Club, and related executables.  
- **Firewall Integration:** Uses Windows `netsh advfirewall` for rule management.  
- **Automatic Privilege Handling:** Detects and requests administrator rights when required.  
- **Configurable Paths:** Manage all executable locations via a `config.json` file.  
- **Built-in Config Editor:** Add, remove, or edit paths directly from the tool.  
- **Readable Terminal UI:** Clear color-coded interface for better visibility and feedback.  
- **Non-destructive:** Does not modify game or system files.  

---

## Configuration
All executable paths are defined in `config.json`.  
This file is generated automatically on first launch and can be edited manually or through the integrated editor.

**Default configuration example:**
```json
{
    "paths": {
        "GTA5": [
            "D:\\SteamLibrary\\steamapps\\common\\Grand Theft Auto V\\GTA5.exe"
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
