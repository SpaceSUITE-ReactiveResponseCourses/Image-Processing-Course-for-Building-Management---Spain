# QGIS 3.28 LTR – Installation Guide

This guide provides instructions for installing **QGIS 3.28 LTR (Long-Term Release)** on Windows, macOS, and Ubuntu/Debian Linux.  
The LTR version is recommended for training, teaching, and production workflows due to its stability and extended support.

---

## 1. Windows Installation (QGIS 3.28 LTR)

### Step 1 — Download the Installer
1. Open a web browser and go to: https://qgis.org/download/
2. Locate the **Long Term Release (LTR)** section.
3. Download the **Standalone Installer** for Windows.

### Step 2 — Install QGIS
1. Locate the downloaded installer file (typically in your Downloads folder).
2. Double-click the file to launch the installation wizard.
3. Accept the license agreement.
4. Keep the default installation settings unless you have specific requirements.
5. Wait for installation to complete.

### Step 3 — Launch QGIS
1. Open the Start Menu.
2. Search for and open:
   **QGIS Desktop 3.28 LTR**

---

## 2. macOS Installation (QGIS 3.28 LTR)

### Step 1 — Download the Installer
1. Go to: https://qgis.org/download/
2. Under **Long Term Release (LTR)**, download the `.dmg` installer for macOS.

### Step 2 — Install QGIS
1. Open the `.dmg` file.
2. Drag the **QGIS** application into the **Applications** folder.

### Step 3 — Launch QGIS
1. Open **Applications**.
2. Double-click **QGIS** to start.

### Step 4 — macOS Security (If Blocked on First Launch)
If macOS warns that the application cannot be opened:
1. Open **System Settings → Security & Privacy → General**
2. Click **Allow Anyway**
3. Launch QGIS again.

---

## 3. Ubuntu / Debian Linux Installation (QGIS 3.28 LTR)

Use the commands below.  
All steps are included inside one code block for convenience.

```bash
# 1. Install required tools
sudo apt install gnupg software-properties-common

# 2. Add the QGIS package signing key
sudo mkdir -m755 -p /etc/apt/keyrings
sudo wget -O /etc/apt/keyrings/qgis-archive-keyring.gpg https://download.qgis.org/downloads/qgis-archive-keyring.gpg

# 3. Add the QGIS LTR repository
# Replace 'jammy' with your Ubuntu/Debian codename (e.g., focal, bullseye, noble)
echo "deb [signed-by=/etc/apt/keyrings/qgis-archive-keyring.gpg] https://qgis.org/ubuntu-ltr jammy main" | sudo tee /etc/apt/sources.list.d/qgis-ltr.list

# 4. Update package lists
sudo apt update

# 5. Install QGIS (and optional GRASS support)
sudo apt install qgis qgis-plugin-grass

# 6. Launch QGIS
qgis
