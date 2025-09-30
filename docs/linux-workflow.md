# Linux Workflow — LG Octane Analysis

This guide outlines the planned workflow for analyzing backups and dumps from the LG Octane (VN530) on Linux (Arch).  
**Focus:** Safe, non-destructive exploration using open-source tools.

---

## 1. Why Linux?

- Open-source tools provide powerful analysis options.
- Safe environment for inspecting firmware or backups without writing to the phone.
- Supports automation with scripts for reproducible workflows.

---

## 2. Tools to Use

- `binwalk` — extract and inspect firmware/binary blobs.
- `xxd` / `hexdump` — view files in hexadecimal.
- `radare2` / `Ghidra` — disassemble firmware or binaries.
- `strings` — extract readable text from files.
- `sha256sum` / `md5sum` — verify integrity of backups/dumps.

---

## 3. Placeholder Scripts

Create dummy scripts in `analysis/` for testing commands:

```bash
#!/bin/bash
# Extract a dummy binary safely
binwalk -e dummy_file.bin
