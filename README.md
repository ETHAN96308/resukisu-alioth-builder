# ReSukiSU + SUSFS Kernel Builder for Mi 11X (alioth)

Automated GitHub Actions CI to build a **ReSukiSU (rsuntk/KernelSU) + SUSFS** patched kernel for the **Xiaomi Mi 11X / POCO F3 / Redmi K40** (`alioth`) running **MIUI OS1.0.4.0.TKHINXM** (Android 13, kernel 4.19.157 non-GKI).

## 🚀 How to Build

1. **Fork or push** this repo to your GitHub account
2. Go to the **Actions** tab
3. Click **"Build ReSukiSU + SUSFS Kernel for alioth"**
4. Click **"Run workflow"** (default settings are pre-configured)
5. Wait ~30-45 minutes
6. Download the **AnyKernel3 flashable zip** from the workflow's Artifacts

## 📱 How to Flash

1. **Backup** your boot partition in TWRP first
2. Copy the zip to your phone storage
3. Boot to recovery (TWRP/OrangeFox)
4. Flash the zip → Reboot
5. Install **ReSukiSU Manager v3.0.1** APK from [rsuntk/KernelSU releases](https://github.com/rsuntk/KernelSU/releases)
6. Install **SUSFS module** from [sidex15/susfs4ksu-module releases](https://github.com/sidex15/susfs4ksu-module/releases) via the Manager

## ⚠️ Important

- **Unlock bootloader** and install **custom recovery** before flashing
- **Always backup** your boot partition first
- If bootloop: restore boot backup in recovery, or `fastboot flash boot stock_boot.img`
- This kernel is built from community sources and should be tested carefully

## 📋 Device Info

| Property | Value |
|---|---|
| Device | Xiaomi Mi 11X / POCO F3 / Redmi K40 |
| Codename | alioth / aliothin |
| SoC | Snapdragon 870 (SM8250-AC / kona) |
| Kernel | 4.19.157 (non-GKI) |
| Android | 13 |
| MIUI | OS1.0.4.0.TKHINXM |
