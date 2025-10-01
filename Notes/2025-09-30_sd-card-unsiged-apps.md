# 2025-09-30 — SD Card Unsigned App Probe on LG Octane VN530

## Why I’m Doing This
I want to see how the phone reacts if I place unsigned BREW app files on the SD card. This helps me figure out where signature enforcement happens.

## Stuff I Used
- Windows 11 (for file prep)
- Arch Linux (for staging files)
- LG Octane VN530 (SW version ZV8)
- microSD 32 GB (FAT32 formatted)
- Files: `HelloUnsigned.mod`, `HelloUnsigned.mif`, `log.txt`

## What I Did
1. Compiled/staged `HelloUnsigned.mod` and `.mif` on Arch.
2. Copied them to the SD card under `/apps/HelloUnsigned/`.
3. Inserted the card into the Octane and checked with the phone’s file manager.
4. Tried to move the files into internal folders.
5. Rebooted the phone to trigger a BREW rescan.
6. Checked if the app appeared in the menu.

## What Happened
- Files were visible on the SD card.
- The phone’s file manager only allowed moving files into media folders, not BREW directories.
- After reboot, the app did not appear in the menu.
- The `.mod` and `.mif` stayed on the SD card; they weren’t deleted.

## What I Learned
- The SD card works as a shuttle for files but not as an installer.
- BREW’s AMS/security module controls signature enforcement and app enumeration.
- To test unsigned apps, I’ll need DIAG/EFS access with BitPim or QPST.

## Next Things to Try
- Use BitPim/QPST to place `.mod`/`.mif` into `/brew/ams/HelloUnsigned/`.
- Drop a harmless text file into internal BREW dirs to see if it gets deleted at boot.
- Write a BREW app that logs to SD to confirm write access once bypass works.
- Begin mapping AMS signature check offsets in ZV8 firmware.

## References / Links
- My GitHub repo: [LG-Octane-Jailbreak-Fixed](https://github.com/TheNoob143/LG-Octane-Jailbreak-Fixed)
- BREW SDK docs (archived)
- BitPim and QPST documentation
