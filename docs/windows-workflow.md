# Windows Workflow — LG Octane (VN530) Exploration

This guide outlines the planned workflow for safely connecting and exploring the LG Octane on a Windows PC.  
**Focus:** Non-destructive backups, media extraction, and preparation for Linux analysis.

---

## 1. Required Computer

- **Windows PC** — needed for:
  - LG/Qualcomm USB drivers
  - BitPim (media and contacts backup)
  - QPST / LGNPST (optional read-only NV or system dumps)

> Linux will be used later for detailed analysis of files and firmware.

---

## 2. Tools to Use

- **BitPim** — backup contacts, SMS, ringtones, wallpapers, and media.
- **Qpst / LGNPST** — optional, for read-only memory dumps.
- **USB cable** compatible with LG Octane.
- **Qualcomm / LG USB drivers** — required for phone detection.

---

## 3. Connect the Phone

1. Plug the LG Octane into your Windows PC via USB.  
2. On the phone, select **Mass Storage / File Transfer** mode if prompted.  
3. Open **Device Manager** → verify the phone appears under **Portable Devices** or **COM Ports**.

---

## 4. Backup Media Safely

1. Launch **BitPim** and select device: **LG Octane VN530**.  
2. Create a local backup folder, e.g.:  
