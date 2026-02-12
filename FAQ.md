# ❓ Frequently Asked Questions (FAQ)

---

## Installation & Setup

### Q: Should I use Windows 10 or Windows 11?
**A:** 
- **Windows 11** recommended for Macs 2016 or newer (better support, longer updates)
- **Windows 10** for older Macs 2011-2015 (more compatible, still works great)
- Both work fine on Boot Camp
- Windows 10 support ends October 2025
- Windows 11 support continues until 2026+

### Q: Can I use this on Apple Silicon (M1/M2/M3/M4)?
**A:** No. Boot Camp only works on **Intel Macs**. Apple Silicon users need virtual machines like Parallels Desktop or UTM. See [README.md](README.md) for details.

### Q: How much disk space do I need?
**A:** At least **64 GB**, preferably **128 GB+**. This includes:
- Windows OS: ~30 GB
- Updates: ~10-15 GB
- Applications & files: remainder

### Q: Do I need a valid Windows product key?
**A:** Yes, for permanent activation. You can install without one, but you'll get watermarks and limited features. Buy from microsoft.com or authorized retailers.

### Q: How long does installation take?
**A:** Usually **30-60 minutes**:
- Partitioning: 5 minutes
- Windows installation: 20-30 minutes
- Driver installation: 5-10 minutes
- Windows updates: 10-20 minutes

### Q: Can I resize the Windows partition later?
**A:** **Not easily.** Plan your partition size carefully before installation. To resize, you'd need to back up and reinstall.

---

## Performance & Usage

### Q: Will Windows run at full speed?
**A:** Yes! Boot Camp is **native installation**, so Windows runs at full Mac hardware speed. No performance penalty.

### Q: Why is Windows so slow after installation?
**A:** Likely **Windows Update** running in background. Let it complete (1-2 hours). Check **Settings → Update & Security**.

### Q: Can I uninstall Windows later?
**A:** Yes, using Boot Camp Assistant:
1. **Finder → Applications → Utilities → Boot Camp Assistant**
2. Click **Restore** (or Remove Partition)
3. Mac reclaims the disk space

### Q: Can I use both macOS and Windows at the same time?
**A:** No. Boot Camp is **dual-boot only** — you must restart to switch. For simultaneous use, use a virtual machine (Parallels/UTM).

### Q: What about gaming?
**A:** Boot Camp supports gaming well:
- Older games: ✅ Works great
- Modern games (GeForce NOW, Game Pass): ✅ Works
- Some new AAA titles: ⚠️ May have driver issues
- Check compatibility before buying

---

## Activation & Licensing

### Q: My product key doesn't work. What do I do?
**A:** 
- Verify you entered it correctly (25 characters, dashes matter)
- Ensure you're using the **correct Windows version** key:
  - Windows 10 key for Windows 10 installation
  - Windows 11 key for Windows 11 installation
  - Keys are not interchangeable between versions!
- Keys from other computers won't work
- Wait 24 hours — Microsoft validates in background
- Contact Microsoft Support if still failing

### Q: Can I use a Windows key from a used computer?
**A:** No. Keys are tied to one computer. You need your own valid license.

### Q: Can I move my Windows to a different Mac?
**A:** Your Windows license is tied to that specific Mac hardware. Moving requires a new Windows license.

### Q: Is Windows Activation required?
**A:** No, but without it:
- Watermark appears on desktop
- Some features disabled
- Occasional notifications

---

## Drivers & Hardware

### Q: What if Boot Camp drivers don't install?
**A:** 
1. Restart your Mac (reboot to Windows first)
2. Manually run `BootCampSetup64.exe` from Windows
3. If still failing, update from Windows Update:
   - **Settings → Update & Security → Check for updates**

### Q: Will my trackpad work?
**A:** Only after installing Boot Camp drivers. Without them:
- Trackpad doesn't respond
- Install drivers (Step 6 in [README.md](README.md))
- Restart
- Trackpad should work

### Q: Why is my display dark/bright levels off?
**A:** Missing graphics drivers. Install Boot Camp drivers to fix brightness controls.

### Q: What about USB devices?
**A:** Most USB devices work out of the box. Printers may need drivers. Install from device manufacturer's website.

---

## Troubleshooting

### Q: Boot Camp Assistant won't open
**A:**
- Restart your Mac
- Try in Recovery Mode: **Cmd + R → Utilities → Boot Camp Assistant**
- Check if your Mac supports Boot Camp (Intel only)

### Q: Windows partition disappeared
**A:**
- Restart and hold **Option (⌥)** during startup
- Windows partition should appear
- If not, you may need to reinstall

### Q: Can't see Windows when restarting
**A:**
- Restart and hold **Option (⌥)** immediately
- You should see **Macintosh HD** and **Windows** options
- Click **Windows** → Enter
- If Windows doesn't appear, try again on next restart

### Q: I accidentally deleted Windows partition
**A:**
- Bad news: Windows installation is lost
- You'll need to reinstall using Boot Camp Assistant
- Your Mac files are safe (they're on macOS partition)

### Q: Windows asks for a product key on every restart
**A:**
- You haven't activated Windows yet
- Go to **Settings → System → About**
- Click **Change product key** or **Activate**
- Enter your key and wait 24-48 hours

### Q: Internet not working in Windows
**A:**
- Install Boot Camp drivers (includes network drivers)
- Or download Ethernet drivers from Apple
- Restart after installation

---

## macOS-Specific

### Q: What's the best macOS version for Boot Camp?
**A:** 
- **macOS Big Sur (11) or later**: Recommended and stable
- **macOS Monterey (12)**: Works well
- **macOS Ventura (13)**: Works well
- **macOS Sonoma (14)+**: Works, fully tested
- Avoid very old versions (pre-Big Sur); support may be limited

### Q: Should I disable FileVault before installing?
**A:** Yes! FileVault encryption can interfere with Boot Camp. Disable it before installation, then re-enable on macOS if desired.

### Q: Can I Time Machine backup Windows?
**A:** Yes, Time Machine backs up the entire Mac including Windows partition. Your backup includes Windows and can be restored.

---

## Pricing & Licensing

### Q: How much does Boot Camp cost?
**A:** **Free!** It's built into every Intel Mac. You only pay for Windows license.

### Q: How much does Windows cost?
**A:** 
- **Windows 11 Home**: ~$140 USD
- **Windows 11 Pro**: ~$200 USD
- **Windows 10 Home**: ~$120 USD (being phased out)
- **Windows 10 Pro**: ~$200 USD
- Often included free or discounted with new computers
- Both available from microsoft.com or authorized retailers

### Q: Can I upgrade from Windows 10 to Windows 11 on unsupported hardware?
**A:** Yes! If your Mac doesn't meet Windows 11 requirements (TPM 2.0, newer CPU), you can bypass these checks. See **[bypass windows 10 to windows 11.md](bypass%20windows%2010%20to%20windows%2011.md)** for step-by-step instructions.

### Q: Can I use Windows 10 on newer Macs?
**A:** Yes, on Intel Macs. But **Windows 11 is recommended** for better compatibility.

---

## Still Have Questions?

Check the **[detailed README.md](README.md)** or contact:
- **Microsoft Support:** support.microsoft.com
- **Apple Support:** support.apple.com/boot-camp

---

**Last Updated:** February 2026
