# 🔓 Bypass Windows 11 System Requirements (Upgrade from Windows 10)

This guide helps you upgrade from Windows 10 to Windows 11 on unsupported hardware (older CPUs, no TPM 2.0, etc.).

---

## ⚠️ Before You Start

- **Back up your data** (critical!)
- You need a valid Windows 10 installation
- Windows 11 ISO downloaded from microsoft.com
- This works for upgrades, not clean installs on Mac Boot Camp

---

## 🛠️ Method 1: Registry Edit (Easiest)

### Step 1: Download Windows 11 ISO
1. Go to https://www.microsoft.com/software-download/windows11
2. Download **Windows 11 ISO (x64)**

### Step 2: Mount the ISO
1. Right-click the ISO file
2. Click **Mount**
3. Note the drive letter (e.g., D:)

### Step 3: Edit Registry
1. Press **Windows Key + R**
2. Type `regedit` and press Enter
3. Navigate to: `HKEY_LOCAL_MACHINE\SYSTEM\Setup\MoSetup`
4. Right-click **MoSetup** → New → **DWORD (32-bit) Value**
5. Name it: `AllowUpgradesWithUnsupportedTPMOrCPU`
6. Double-click it and set value to **1**
7. Close Registry Editor

### Step 4: Run Setup
1. Open File Explorer
2. Go to mounted ISO drive
3. Run **setup.exe**
4. Follow installation prompts
5. Windows 11 will install, bypassing checks

---

## 🛠️ Method 2: Rufus USB (Alternative)

### Step 1: Download Rufus
- Get Rufus from https://rufus.ie

### Step 2: Create Bootable USB
1. Insert USB drive (8 GB+)
2. Open Rufus
3. Select Windows 11 ISO
4. Check: **Remove requirement for 4GB+ RAM, Secure Boot and TPM 2.0**
5. Click **Start**

### Step 3: Boot from USB
1. Restart PC
2. Boot from USB
3. Install Windows 11 normally

---

## 🛠️ Method 3: In-Place Upgrade Script

Run this in Command Prompt (Admin):

```cmd
reg add HKLM\SYSTEM\Setup\MoSetup /v AllowUpgradesWithUnsupportedTPMOrCPU /t REG_DWORD /d 1 /f
```

Then run setup.exe from Windows 11 ISO.

---

## ✅ Verify Upgrade

After installation:
1. Press **Windows Key + I**
2. Go to **System → About**
3. Check **Windows specifications** shows Windows 11

---

## ⚠️ Known Issues

- Windows Update may show warnings about unsupported hardware
- Some features may not work (e.g., Android apps, certain security features)
- Future updates may be blocked (rare)

---

## 🔄 Rollback to Windows 10

If you want to go back (within 10 days):
1. **Settings → System → Recovery**
2. Click **Go back** under "Recovery options"
3. Follow prompts

---

**Last Updated:** February 2026
