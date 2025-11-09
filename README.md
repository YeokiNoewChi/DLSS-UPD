# DLSS-UPD

DLSS-UPD is a lightweight Windows application that helps you manage and update NVIDIA DLSS files quickly and safely.  
It provides an easy-to-use interface for checking, updating, and rolling back DLSS versions without needing to browse game folders manually.

---

## Installation

DLSS-UPD includes an **Inno Setup installer** for a straightforward installation process.

1. Download the latest **DLSS-UPD Installer (.exe)** from the Releases page.  
2. Run the installer and follow the on-screen instructions.  
3. Choose your preferred installation directory (default: `C:\Program Files\DLSS-UPD`).  
4. Once the installation completes, launch the program from the desktop shortcut or Start Menu.

### Safety Notice

Because DLSS-UPD is a small open-source application, **Windows SmartScreen** may show a warning like:  
> *“Windows protected your PC.”*

This message appears for most unsigned software.  
To proceed safely:

1. Click **More Info**  
2. Select **Run Anyway**

DLSS-UPD does **not** contain any harmful or malicious code.  
It only accesses your local game files and checks online for DLSS updates.

---

## Uninstallation

To remove DLSS-UPD from your system:

1. Open the **Control Panel** or **Settings → Apps**  
2. Locate **DLSS-UPD** in the installed applications list  
3. Click **Uninstall** and follow the prompts  

Alternatively, you can run `unins000.exe` located in your installation directory (default:  
`C:\Program Files\DLSS-UPD`) to remove it completely.

All program files and shortcuts will be deleted safely.

---

## How to Use

1. Open **DLSS-UPD**  
2. Select your game folder or drag and drop it into the window  
3. Click **Scan** to detect your current DLSS version  
4. Click **Update** to install the latest DLSS release  
5. Use **Rollback** if you want to return to a previous version  

All updates are verified locally, and logs are automatically saved for reference.

---

## Features

- Detects installed DLSS versions  
- Updates to the latest available builds  
- Rolls back to earlier versions when needed  
- Supports drag-and-drop folder selection  
- Displays progress during updates  
- Generates logs for transparency  

---

## Requirements

- Windows 10 or newer  
- .NET 6.0 or later  
- Internet connection (for version checks and downloads)

---

## Technical Overview

DLSS-UPD is written in **C#** using **WPF (XAML)**.  
It’s designed with simplicity, reliability, and maintainability in mind.

Highlights:

- Organized XAML structure and custom control templates  
- Clean data binding with lightweight converters  
- Minimal code-behind logic for performance and clarity  

To build from source:

```bash
git clone https://github.com/<your-repo>/DLSS-UPD.git
cd DLSS-UPD
dotnet build
