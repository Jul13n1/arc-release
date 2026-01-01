# Arc Agent Installer

```
  █████╗  ██████╗  ██████╗ 
 ██╔══██╗██╔══██╗██╔════╝ 
 ███████║██████╔╝██║      
 ██╔══██║██╔══██╗██║      
 ██║  ██║██║  ██║╚██████╗ 
 ╚═╝  ╚═╝╚═╝  ╚═╝ ╚═════╝ 
```


This repository hosts the official installer and release artifacts for the **Arc Agent**.

> **Arc** is a secure, cross-platform active relay cluster for virtualising and sharing USB devices over a network.

## 🚀 Download & Install

### Option 1: Winget (Recommended)

The easiest way to install Arc is via the Windows Package Manager (Winget). Open PowerShell or Command Prompt and run:

```powershell
winget install jul13n1.ArcAgent
```

To update to the latest version:

```powershell
winget upgrade jul13n1.ArcAgent
```

### Option 2: Manual Download

1.  Go to the [**Releases**](../../releases) page.
2.  Download the latest `Arc_Installer_x.x.x_windows.exe`.
3.  Run the installer.

## ✨ Installer Features

This installer is an **all-in-one** package that sets up everything you need to share and connect to USB devices:

- **Arc Agent**: The core client application.
- **USBIPD-WIN**: Installs the server-side drivers (required for sharing local USB devices).
- **USBIP-WIN2**: Installs the client-side drivers (required for attaching remote USB devices).
- **Service Management**: Utilities to run Arc as a background service.

> [!NOTE]
> The installer requires **Administrator privileges** to install the necessary drivers. A system reboot may be required after installation to ensure all drivers are loaded correctly.

## ✨ Agent Features

The Arc Agent provides a powerful set of tools for seamless device sharing:

*   **USB Device Sharing**: Easily share local USB devices (dongles, keys, specialised hardware) over the network.
*   **Remote Attachment**: Connect to devices shared by other agents in your organisation as if they were plugged into your machine.
*   **Virtualisation**: Uses native OS virtualisation (USBIP) for high compatibility and performance.
*   **Secure Access**: Group-based isolation and token authentication ensure only authorised users can access sensitive devices.
*   **Service Mode**: Run Arc as a background Windows service for always-on availability, independent of user sessions.
*   **Modern UI**: stunning, hardware-accelerated interface with dark mode, animations, and glassmorphism effects.
*   **Device Aliasing**: Rename devices with friendly aliases for easier identification.
*   **Resilient Connections**: Automatic reconnection and error recovery handling for unstable networks.
*   **Queuing System**: Request access to busy devices and get notified when they become available.

## � Built With

Arc is built using modern, high-performance technologies:

*   **Go (Golang)**: Core agent logic, networking, and device management.
*   **Vue.js 3**: Client Admin UI with reactive state management.
*   **Vite**: Fast build tool and development server.
*   **USBIP**: Industry-standard USB-over-IP protocol for reliable device virtualization.

## �🛠️ Usage

Once installed:

1.  Launch **Arc Agent** from the Start Menu or Desktop.
2.  The Arc icon will appear in your **System Tray**.
3.  Right-click the tray icon to **Open Web Interface**.
4.  From the Agent UI, you can:
    -   **Manage Devices**: Share and attach USB devices.
    -   **Check for Updates**: Easily upgrade to the latest version.
    -   **Exit**: Close the agent completely.

## 🔗 Links

- **Source Code**: [Jul13n1/arc](https://github.com/Jul13n1/arc) - The main repository containing the source code for the Agent, Server, and Admin UI.
- **Issues**: [Jul13n1/arc/issues](https://github.com/Jul13n1/arc/issues) - Report bugs or request features.

## 🛑 Support

If you encounter issues during installation:

1.  Ensure you ran the installer as Administrator.
2.  If driver installation fails, you can try installing them manually:
    - [usbipd-win](https://github.com/dorssel/usbipd-win)
    - [usbip-win2](https://github.com/vadimgrn/usbip-win2)
