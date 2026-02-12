# 🔓 Bypass Windows 11 System Requirements (Upgrade from Windows 10)

This guide helps you upgrade from Windows 10 to Windows 11 on unsupported hardware (older CPUs, no TPM 2.0, Secure Boot, etc.).

---

## ⚠️ Before You Start

- **Back up your data** (critical!)
- You need a valid Windows 10 installation (activated)
- Windows 11 ISO downloaded from microsoft.com
- At least **10 GB free space** on C: drive
- Administrator access to your PC

> ⚠️ **Note:** This works for in-place upgrades. For clean installs on unsupported Macs, see the main README.md.

---

## 🛠️ Method 1: Setup Command Bypass (Easiest & Recommended)

### Step 1: Download Windows 11 ISO
1. Go to https://www.microsoft.com/software-download/windows11
2. Download **Windows 11 ISO (x64)** for Intel Macs
3. Wait for download to complete (~5 GB)

### Step 2: Extract ISO Files
1. **Right-click** the downloaded ISO file
2.  open the file 
4. **Select all files** (Ctrl + A) and **Copy** (Ctrl + C)
5. Open **C: drive** in File Explorer
6. Create a new folder named **win11**
7. Open the **win11** folder and **Paste** (Ctrl + V)
8. Wait for all files to copy (~5-10 minutes)

### Step 3: Run Setup with Bypass Command
1. Press **Windows Key + x**
2. Select **Command Prompt (Admin)** 
3. Type the following command and press **Enter**:
   ```
   c:\win11\setup.exe /product server
   ```
4. Wait for Windows 11 Setup to launch

### Step 4: Install Windows 11
1. Windows 11 Setup window appears
2. Click **Next**
3. Click **Accept** on license terms
4. Choose **Keep personal files and apps** (recommended)
5. Click **Install**
6. Wait for installation (30-60 minutes)
7. Your PC will restart several times (normal)

### Step 5: Clean Up Installation Files
1. After Windows 11 boots successfully
2. Open **File Explorer**
3. Navigate to **C:\win11**
4. **Delete the entire win11 folder** to free up ~5 GB
5. Empty **Recycle Bin**

---


## ✅ Verify Upgrade

After installation:
1. Press **Windows Key + I**
2. Go to **System → About**
3. Check **Windows specifications** shows Windows 11

---

## ⚠️ Known Issues & Limitations

- **Windows Update warnings:** You may see "This PC doesn't meet Windows 11 requirements" (cosmetic only)
- **Missing features:** Android apps, Windows Studio Effects, some security features
- **Future updates:** Major updates (24H2, etc.) may require repeating bypass method
- **Performance:** Runs normally on most hardware despite warnings



## 🆘 Troubleshooting

| Issue | Solution |
|-------|----------|
| **"Setup.exe not found"** | Check path: `c:\win11\setup.exe` exists |
| **"Access denied"** | Run Command Prompt as Administrator |
| **Setup crashes** | Disable antivirus temporarily |
| **"Not enough space"** | Free up 10+ GB on C: drive |
| **Stuck at 0%** | Wait 10-15 minutes, restart if no progress |
| **Black screen after install** | Wait 30 minutes, force restart if needed |

---

## 📚 Additional Resources

- **Microsoft Windows 11 Requirements:** https://www.microsoft.com/windows/windows-11-specifications
- **Windows 11 Support:** https://support.microsoft.com/windows

---

**Last Updated:** February 2025
