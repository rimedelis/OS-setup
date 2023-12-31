# Optimization Checklist for Windows

1. **Check for regular and additional updates!**

2. **Disable/uninstall bloatware and startup apps**

3. **Setup PIN**

4. **Go to Clean recommendations to delete trash files**

5. **Disable all notifications**

6. **Disable all taskbar icons**

7. **Set Power to Best Performance while plugged in and Battery Saver otherwise**

8. **Windows God Mode:** Create a folder called "GodMode.{ED7BA470-8E54-465E-825C-99712043E01C}" that gives us all hidden Windows settings

9. **Change default browser and any other default apps**

10. **Update drivers using Windows Update or trying Device Manager**

11. **Change privacy settings:** General and Diagnostics

12. **Disable a few services built into Windows:** telemetry, print spooler, or geolocation

13. **Enable Clipboard history**

14. **Show hidden files:** Don't hide empty drives or extensions for known file types.

15. **(Optional) Install Wintoys tool by Bogdan P.**

# Installing programs with Chocolatey

1. First, install Chocolatey:

   ```powershell
   Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))
   ```

2. Use this to never be asked for permission to run (always Yes to prompts):

   ```powershell
   choco feature enable -n=allowGlobalConfirmation
   ```

   To disable this:

   ```powershell
   choco feature disable -n=allowGlobalConfirmation
   ```

3. Programs to install:

   ```powershell
   choco install anaconda3 -y
   choco install git -y
   choco install googlechrome -y
   choco install mingw -y
   choco install microsoft-windows-terminal -y
   choco install msys2 -y
   choco install nodejs.install -y
   choco install python -y
   choco install qbittorrent -y
   choco install ruby -y
   choco install vscode -y
   choco install wsl2 --params "/Version:2 /Retry:true" -y
   ```

# Install Ruby On Rails on Windows 11: [GoRails Setup](https://gorails.com/setup/windows/11)

Other programs with Chocolatey:

   ```powershell
   choco install sonicpi -y
   choco install vmware-workstation-player -y
   choco install ngrok -y
   choco install gramps -y
   choco install thonny -y
   ```

Other programs not available with Chocolatey:

- UltraStar Deluxe
