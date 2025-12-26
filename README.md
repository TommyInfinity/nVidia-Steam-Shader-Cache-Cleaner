# 🎮 NVIDIA & Steam Shader Cache Cleaner

A simple Windows desktop application for cleaning NVIDIA DirectX/OpenGL and Steam shader caches to improve gaming performance and free up disk space.

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Platform](https://img.shields.io/badge/platform-Windows-lightgrey.svg)
![.NET](https://img.shields.io/badge/.NET-9.0-purple.svg)

## ✨ Features

- 🔍 **Smart Detection** - Automatically locates NVIDIA and Steam shader cache folders
- 📊 **Size Calculation** - Displays real-time cache sizes in human-readable format
- 🗑️ **Selective Deletion** - Delete individual caches or all at once
- 📁 **Quick Navigation** - Open cache folders directly in Windows Explorer
- 🎨 **Modern Dark UI** - Clean, intuitive interface with smooth animations
- 🛡️ **Admin Support** - Runs with elevated privileges for protected files
- ⚡ **Single Executable** - Portable, no installation required

## 🖼️ Screenshots

<img width="881" height="559" alt="kép" src="https://github.com/user-attachments/assets/04f4b0be-178d-472f-803a-98743adbbc78" />

### Main Interface
The application features a clean, dark-themed interface with clearly separated cache sections:
- DirectX Cache (DXCache)
- OpenGL Cache (GLCache)
- Steam Shader Cache

Each section displays:
- Current folder path
- Total cache size
- Individual delete and navigate buttons

## 🚀 Getting Started

### Prerequisites

- Windows 10/11 (64-bit)
- Administrator privileges (for accessing protected cache folders)

### Installation

1. Download the latest release from the [Releases](../../releases) page
2. Extract the ZIP file to your desired location
3. Run `nVidia Cache Cleaner.exe` as Administrator

**Note:** The application will automatically request administrator privileges on launch.

## 📖 Usage

### Scanning for Caches

1. Click the **🔍 Scan** button to detect all shader cache folders
2. The application will search for:
   - `%LocalAppData%\NVIDIA\DXCache`
   - `%LocalAppData%\NVIDIA\GLCache`
   - Steam shader cache (auto-detected from registry)

### Deleting Caches

**Individual Deletion:**
- Click the **Delete** button next to any cache section
- Confirm the deletion prompt

**Bulk Deletion:**
- Click **🗑️ Delete All** to remove all detected caches at once
- Confirm the bulk deletion prompt

### Navigating to Folders

- Click **📁 Navigate** next to any cache section
- The folder opens in Windows File Explorer
- Only enabled for detected/existing folders

## 🛠️ Technical Details

### Key Features Implementation

- **Registry Reading:** Detects Steam installation path automatically
- **Recursive Deletion:** Safely removes all files and subdirectories
- **Size Calculation:** Efficient directory traversal with error handling
- **Process Launching:** Opens Windows Explorer for folder navigation

### Requirements

- Visual Studio 2022 or later
- .NET 9.0 SDK
- Windows 10/11 SDK


## ⚠️ Important Notes

- **Administrator Rights:** Required for deleting protected cache files
- **Steam Detection:** Automatically searches registry and common installation paths
- **Safe Deletion:** Files are permanently deleted (not moved to Recycle Bin)
- **Performance:** Shader cache regeneration may cause temporary FPS drops after deletion

## 👾 VirusTotal Check

You can scan and check the file here > [Click here](https://www.virustotal.com/gui/file/28708242389e565ac5086ec743e9583a919509ce4571b7ebbb5bd3923969e489)
Also you can upload and check for any virus or malicious stuff yourself [here](https://www.virustotal.com/gui/home/upload).

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Inspired by [NVIDIA-GPU-Shader-Cache-Cleaner](https://github.com/dubbyOW/NVIDIA-GPU-Shader-Cache-Cleaner)
- Built with modern WPF best practices
- UI design influenced by Visual Studio's dark theme

## 📧 Contact

Project Link: [https://github.com/yourusername/nvidia-cache-cleaner](https://github.com/TommyInfinity/nVidia-Steam-Shader-Cache-Cleaner)

---

⭐ If you find this project useful, please consider giving it a star!
