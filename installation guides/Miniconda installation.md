This document contains instructions to install miniconda on your specific OS.

Please find the various steps here:

- [Windows](#Miniconda-Installation-on-Windows)
- [MacOS](#Miniconda-Installation-on-macOS)
- [Linux](#Miniconda-Installation-on-Linux)

### **Miniconda Installation on Windows**

1. Go to the Miniconda download page:  
    https://docs.conda.io/en/latest/miniconda.html
    
2. Under **Windows Installers**, download:
    - **Miniconda3**
    - **64-bit**
    - Installer type: `.exe`
        
3. Once downloaded, double-click the `.exe` file to start the installation.
    
4. In the setup window:
    - Click **Next**.
    - Accept the **license agreement**.
    - Choose **Just Me** (recommended) or **All Users** if you need system-wide access.
    - Keep the default **installation location** unless you have a specific reason to change it.
        
5. On the **Advanced Options** screen:
    - Leave **Add Miniconda to my PATH** **unchecked** (recommended).
    - Leave **Register Miniconda as the system Python** **checked**.
        
6. Click **Install** and wait for the installation to complete.
    
7. Click **Finish**.
    
8. Open the Start Menu and launch:  
    **Miniconda Prompt** (or **Anaconda Prompt**, depending on installer version).
    
9. Verify the installation:
    `conda --version`



### **Miniconda Installation on macOS**
1. Determine your Mac type:
    - Apple Silicon (M1 / M2 / M3) → use the **arm64** installer.
    - Intel → use the **x86_64** installer.
        
2. Go to the Miniconda download page:  
    https://docs.conda.io/en/latest/miniconda.html
    
3. Download the installer that matches your Mac:
    - Apple Silicon: `Miniconda3-latest-MacOSX-arm64.sh`
    - Intel: `Miniconda3-latest-MacOSX-x86_64.sh`
        
4. Open **Terminal** (Applications → Utilities → Terminal).
    
5. Navigate to your Downloads folder:
    `cd ~/Downloads`
    
6. Make the installer executable:
    `chmod +x Miniconda3-latest-MacOSX-*.sh`
    
7. Run the installer:
    `./Miniconda3-latest-MacOSX-*.sh`
    
1. Follow the prompts:
    - Press **Enter** to scroll through the license.
    - Type **yes** to accept the license.
    - Press **Enter** to accept the default install location.
    - Type **yes** to allow the installer to initialize Conda.
        
2. Reload your shell so Conda is recognized:
    `source ~/.zshrc`
    
    (If you use bash instead of zsh, run `source ~/.bashrc`)
    
3. Verify the installation:
    `conda --version`



### **Miniconda Installation on Linux**
1. Open a terminal.
    
2. Download the Miniconda installer (64-bit):
    `wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh`
    
3. Make the installer executable:
    `chmod +x Miniconda3-latest-Linux-x86_64.sh`
    
4. Run the installer:
    `./Miniconda3-latest-Linux-x86_64.sh`
    
5. Follow the prompts:
    - Press **Enter** to scroll through the license.
    - Type **yes** to accept the license.
    - Press **Enter** to confirm the default install location.
    - Type **yes** when asked to initialize Miniconda.
        
6. Reload your shell so Conda is recognized:
    `source ~/.bashrc`
    
    (If your shell is zsh instead, run `source ~/.zshrc`)
    
1. Confirm Miniconda installed correctly:
    `conda --version`
