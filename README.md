# 🐷 CookedHamTweaker v2

> **Crisp your Windows install like bacon, not your telemetry.**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Windows 11](https://img.shields.io/badge/Windows-11-0078D6?logo=windows)](https://www.microsoft.com/windows/windows-11)
[![Windows 10](https://img.shields.io/badge/Windows-10-0078D6?logo=windows)](https://www.microsoft.com/windows/windows-10)
[![PowerShell](https://img.shields.io/badge/PowerShell-5391FE?logo=powershell&logoColor=white)](https://docs.microsoft.com/powershell/)

CookedHamTweaker is an opinionated Windows 11/10 **privacy, debloat, and performance script generator**. It provides a sleek web-based interface to customize and generate PowerShell scripts that optimize your Windows installation.

![CookedHamTweaker Screenshot](<img width="997" height="708" alt="image" src="(https://github.com/porkmagus/CookedHamTweaker/blob/main/screen.png)"/>)

## ✨ Features

- 🔒 **Privacy & Security** — Disable telemetry, advertising ID, Cortana, Recall AI, and more
- ⚡ **Performance Optimization** — Game Mode, HAGS, network throttling, visual effects tuning
- 🔋 **Power Management** — Power plans, hibernation, sleep settings, CPU performance
- 🎨 **UI Customization** — Dark/Light mode, taskbar tweaks, classic context menu (Windows 11)
- ⚙️ **Services Control** — Disable unnecessary Windows services safely
- 🔄 **Windows Updates** — Control update behavior, defer updates, disable P2P delivery
- 🔔 **Notifications** — Silence system notifications, tips, and suggestions
- 🧹 **Bloatware Removal** — Remove pre-installed apps like Cortana, Xbox, Teams, and more

## 🚀 Quick Start

### Option 1: Use Online (Recommended)
Visit the hosted version at: **[Your GitHub Pages URL]**

### Option 2: Run Locally
1. Download or clone this repository
2. Open `index.html` in any modern web browser
3. Select your desired tweaks
4. Download or copy the generated PowerShell script
5. Run the script as Administrator

```powershell
# Run in elevated PowerShell
Set-ExecutionPolicy -ExecutionPolicy Bypass -Scope Process
.\CookedHamTweaker.ps1
```

## 📋 Usage Guide

### Selecting Tweaks

1. **Manual Selection** — Click individual tweaks to enable/disable them
2. **Profiles** — Use preset profiles for common use cases:
   - 🔒 **Hardcore Privacy** — Maximum privacy protection
   - 🎮 **Gaming Focused** — Optimized for gaming performance
   - ⚖️ **Balanced** — A mix of privacy and performance
   - 🚀 **Max Everything** — All tweaks enabled

3. **Search** — Filter tweaks by name or description
4. **Select All Visible** — Enable all currently visible tweaks

### Generating Scripts

- **Copy** — Copy the script to clipboard
- **Download** — Save as `CookedHamTweaker.ps1`
- **Clear** — Reset all selections

## ⚠️ Risk Levels

Some tweaks are marked with **(RISK)** indicating they may:
- Break certain Windows features
- Cause compatibility issues with some applications
- Reduce system security

**Always review the generated script before running!**

### High-Risk Tweaks Include:
| Tweak | Risk |
|-------|------|
| Disable Telemetry | May break Windows Update & Store |
| Lower UAC | Reduces security significantly |
| Disable Windows Search | Breaks Start menu search |
| Disable SysMain | May reduce app launch performance on HDDs |
| Disable Print Spooler | No printing support |
| Disable Auto Updates | Security vulnerabilities |

## 🔧 Tweak Categories

### 🔒 Privacy & Security (40+ tweaks)
- Advertising & tracking controls
- Lock screen privacy
- Speech & voice settings
- Input & typing telemetry
- Diagnostic data controls
- Location services
- Camera & microphone access
- Account sync settings
- Copilot & Recall AI controls

### ⚡ Performance & Gaming (35+ tweaks)
- Game Mode optimization
- GPU scheduling (HAGS)
- Network throttling
- Visual effects optimization
- Memory management
- File system tweaks
- Mouse & keyboard optimization
- NVMe experimental driver

### 🔋 Power Management (17 tweaks)
- Power plan selection
- Fast Startup & Hibernation
- Display & sleep settings
- USB power settings
- CPU performance states

### 🎨 UI & Appearance (30 tweaks)
- Dark/Light mode
- Taskbar customization
- Start menu settings
- File Explorer options
- Classic context menu (Windows 11)

### ⚙️ Services (23 tweaks)
- Xbox services
- Remote services
- Diagnostic services
- Media services
- Sync services

### 🔄 Windows Updates (10 tweaks)
- Update behavior control
- P2P delivery settings
- Feature/Quality update deferral
- Driver update control

### 🔔 Notifications (9 tweaks)
- System notification controls
- Sound scheme settings
- Tips & suggestions

### 🧹 Bloatware Removal (35 apps)
- Microsoft apps (Teams, Cortana, OneDrive)
- Xbox apps
- Pre-installed games
- Utility apps

## 🖥️ System Requirements

- **OS:** Windows 10 (1903+) or Windows 11
- **Browser:** Any modern browser (Chrome, Firefox, Edge)
- **Execution:** PowerShell 5.1+ (Run as Administrator)

## 📁 Project Structure

```
CookedHamTweaker/
├── index.html          # Main application (single file)
├── README.md           # This file
└── LICENSE             # MIT License
```

## 🔐 Security & Privacy

- **No data collection** — Everything runs locally in your browser
- **No external dependencies** — Single HTML file, no CDN calls
- **Open source** — Full transparency, audit the code yourself
- **No installation required** — Just open and use

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. **Fork** the repository
2. **Create** a feature branch (`git checkout -b feature/amazing-tweak`)
3. **Commit** your changes (`git commit -m 'Add amazing tweak'`)
4. **Push** to the branch (`git push origin feature/amazing-tweak`)
5. **Open** a Pull Request

### Adding New Tweaks

Tweaks are defined in the `tweaksData` object. Each tweak has:
```javascript
{
    name: "Tweak Name",           // Display name
    desc: "Description",          // Short description
    cmd: "powershell command",    // PowerShell command(s)
    risk: true                    // Optional: marks as risky
}
```

## 📜 Changelog

### v2.0.0
- 🐷 Major update with HamTweak.ps1 integration
- 🔒 Privacy & Security tweaks
- ⚡ Performance optimizations
- 🔋 Power management tweaks
- 🎨 UI & Visual customizations
- ⚙️ Windows Services control
- 🔄 Windows Updates settings
- 🔔 Notification tweaks
- 🧹 Bloatware removal

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## ⚖️ Disclaimer

**USE AT YOUR OWN RISK.** This tool modifies Windows system settings and registry entries. While all tweaks have been tested, the author is not responsible for any damage, data loss, or system instability that may occur. Always:

- ✅ Create a system restore point before running
- ✅ Backup important data
- ✅ Review the generated script before execution
- ✅ Understand what each tweak does

## 🙏 Acknowledgments

- Inspired by various Windows optimization tools and privacy guides
- Built with vanilla HTML, CSS, and JavaScript
- No frameworks, no dependencies, just pure web tech

---

<p align="center">
  Made with 🐷 by <a href="https://github.com/porkmagus">porkmagus</a>
  <br>
  <a href="https://github.com/porkmagus/CookedHamTweaker">⭐ Star this repo if you found it useful!</a>
</p>




