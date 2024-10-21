# $\color{white}{\textbf{WSL - Windows Subsystem for Linux} \text{🐧}}$

<img src="https://github.com/user-attachments/assets/aaeed8ed-65a0-4495-a906-3ad85db3aff8" alt="WSL Logo" width="700"/>

$\color{lightgray}{\text{WSL (Windows Subsystem for Linux) allows you to run Linux distributions natively on Windows 10 and Windows 11, enabling developers to use a Linux environment alongside their Windows applications.} \text{🌟}}$

---

## $\color{cyan}{\textbf{Key Features} \text{🌟}}$

- $\color{lightblue}{\textbf{Run Linux Distributions}}$: Seamlessly run distributions like Ubuntu, Debian, and more.
- $\color{lightblue}{\textbf{Windows and Linux Integration}}$: Use Windows tools alongside Linux command-line tools. $\text{🔄}$
- $\color{lightblue}{\textbf{File Management}}$: Easily access both Windows and Linux file systems. $\text{📁}$
- $\color{lightblue}{\textbf{Support for Docker}}$: Run Docker containers in a Linux environment. $\text{🐳}$
- $\color{lightblue}{\textbf{High Performance}}$: Fast execution without the overhead of a full virtual machine. $\text{⚡}$

---

## $\color{cyan}{\textbf{Installation Guide} \text{🛠️}}$

### $\color{orange}{\textbf{Prerequisites} \text{✅}}$

- $\color{lightgray}{\textbf{Windows 10 (Version 1903 or higher) or Windows 11.}}$
- $\color{lightgray}{\textbf{Virtualization must be enabled in your BIOS.}}$

### $\color{orange}{\textbf{Installation Steps} \text{🚀}}$

1. **Open PowerShell**:
   - Right-click on the Start menu and select **Windows PowerShell (Admin)**.

2. **Install WSL**:
   - Run the following command to install WSL and the default Linux distribution:
     ```bash
     wsl --install
     ```

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
   - After enabling features, restart your computer. $\text{🔄}$

6. **Install a Linux Distribution**:
   - Open the **Microsoft Store** and search for your preferred distribution (e.g., **Ubuntu**). Click **Install**. $\text{📥}$

7. **Set WSL Version to 2**:
   - To set WSL to version 2, use this command:
     ```bash
     wsl --set-default-version 2
     ```

---

## $\color{cyan}{\textbf{User Guide} \text{📚}}$

### $\color{lightblue}{\textbf{Running WSL}}$

- Launch your installed Linux distribution by typing the following command in **Command Prompt** or **PowerShell**:
  ```bash
  wsl
### $\color{lightblue}{\textbf{Run as Root}}$

- To run WSL as the **root** user, use:
  ```bash
  wsl -u root                  

### $\\color{cyan}{\\textbf{Integrations with Other Tools} \\text{🔗}}$

| $\\color{lightblue}{\\textbf{Application}}$              | $\\color{lightblue}{\\textbf{Description}}$                                             | $\\color{lightblue}{\\textbf{Link}}$                      |
|----------------------------------------------------------|-----------------------------------------------------------------------------------------|-----------------------------------------------------------|
| Docker                                                   | Manage containers and run multiple apps on Linux                                       | [Visit Docker](https://www.docker.com/) $\\text{🐳}$      |
| Visual Studio Code                                       | Powerful IDE with WSL support                                                          | [Visit VS Code](https://code.visualstudio.com/) $\\text{💻}$ |



### $\\color{cyan}{\\textbf{Troubleshooting} \\text{🛠️}}$

| $\\color{lightblue}{\\textbf{Issue}}$                       | $\\color{lightblue}{\\textbf{Solution}}$                                                   |
|-------------------------------------------------------------|--------------------------------------------------------------------------------------------|
| WSL not starting                                            | Ensure WSL and Virtual Machine Platform are enabled. Restart your computer. $\\text{🔄}$   |
| Distribution not working                                    | Update the distribution: `sudo apt update && sudo apt upgrade`                            |
| Failed to upgrade to WSL 2                                  | Check BIOS settings for virtualization support.                                           |


### $\\color{cyan}{\\textbf{Additional Resources} \\text{📖}}$

- [Official WSL Documentation](https://docs.microsoft.com/en-us/windows/wsl/)
- [WSL Installation Guide by Microsoft](https://docs.microsoft.com/en-us/windows/wsl/install)







