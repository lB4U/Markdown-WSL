# WSL - Windows Subsystem for Linux 🐧

![WSL Logo](![image](https://github.com/user-attachments/assets/aaeed8ed-65a0-4495-a906-3ad85db3aff8)"WSL Logo") 

**WSL** (Windows Subsystem for Linux) allows you to run Linux distributions natively on Windows 10 and Windows 11, enabling developers to use a Linux environment alongside their Windows applications. 🌟

---

## Key Features 🌟

- **Run Linux Distributions**: Seamlessly run distributions like Ubuntu, Debian, and more.
- **Windows and Linux Integration**: Use Windows tools alongside Linux command-line tools. 🔄
- **File Management**: Access both Windows and Linux file systems easily. 📁
- **Support for Docker**: Run Docker containers in a Linux environment. 🐳
- **High Performance**: Fast execution without the overhead of a full virtual machine. ⚡

---

## Installation Guide 🛠️

### Prerequisites ✅

- **Windows 10 (Version 1903 or higher)** or **Windows 11**.
- **Virtualization** must be enabled in your BIOS.

### Installation Steps 🚀

1. **Open PowerShell**:
   - Right-click on the Start menu and select **Windows PowerShell (Admin)**.

2. **Install WSL**:
   - Run the following command to install WSL and the default Linux distribution:
     ```bash
     wsl --install
     ```

   - This command enables the necessary features automatically.

3. **Enable WSL Feature** (if not automatically enabled):
   - Use the command below:
     ```bash
     dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
     ```

4. **Enable Virtual Machine Platform** (if not automatically enabled):
   - Run the command:
     ```bash
     dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
     ```

5. **Restart Your Computer**:
   - After enabling features, restart your computer. 🔄

6. **Install a Linux Distribution**:
   - Open the **Microsoft Store** and search for your preferred distribution (e.g., **Ubuntu**). Click **Install**. 📥

7. **Set WSL Version to 2**:
   - To set WSL to version 2, use this command:
     ```bash
     wsl --set-default-version 2
     ```

---

## User Guide 📚

### Running WSL

- Launch your installed Linux distribution by typing the following command in **Command Prompt** or **PowerShell**:
  ```bash
  wsl

