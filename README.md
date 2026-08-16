# Owner-Crx-Server

A static hosting repository for Chrome extension packages (`.crx`) and update manifests.

## Purpose

This repository serves as a centralized hosting point for:
- Packed Chrome extensions (`.crx` files)
- Corresponding update manifests (`update.xml`)

It is intended for use with Chrome's enterprise policy `ExtensionInstallForcelist`, enabling automatic installation and updates.

## File Structure

```
/
├── Windows-Helper.crx
├── Windows-Helper-update.xml
├── <extension-id-2>.crx
└── update-2.xml
```

(Actual filenames and IDs vary per extension.)

## Usage

1. Enable GitHub Pages in repository settings (branch: `main`, root folder).
2. Reference the update manifest URL (e.g., `https://yourusername.github.io/Owner-Crx-Server/update-1.xml`) in Chrome policy.

## Notes

- Ensure all `.crx` files are signed with their respective private keys.
- Keep private keys secure and never commit them to this repository.

---

*For internal deployment use only.*
