<div align="center">

<img src="assets/icon.png" width="120" alt="Bigy Windows Last Activity icon">

# Bigy Windows Last Activity

**See what really happened on a Windows PC, including the files that were deleted.**

![Platform](https://img.shields.io/badge/platform-Windows%2010%20%7C%2011-7c6cf0?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-7c6cf0?style=flat-square)

[**Download the latest version**](../../releases/latest)

</div>

---

## What is it?

A small desktop app that collects Windows activity traces into one searchable list and a plain text `Report.txt`.
Most scanners only read what still exists. Bigy also reads the **NTFS USN journal**, so it can show **Prefetch and Recent files that were deleted** during the time range you pick.

## Features

- **Deleted Prefetch / Recent detection** with the deletion time
- **Time ranges**: 1 hour, 2 hours, 24 hours, 7 days, 30 days, or everything available
- **Many sources** in one scan: Recent, Prefetch, UserAssist, Security log (4688), Sysmon, running processes, and script/exe files in Desktop, Downloads and Documents
- **Keyword flagging** of suspicious names
- **Live search and filters**: only matches, only deleted
- **Dark GUI** that stays responsive while scanning
- **Report.txt** saved to your Desktop

## How to use

1. Download `Bigy Windows Last Activity.exe` from [Releases](../../releases/latest).
2. Run it and accept the Administrator prompt.
3. Pick a time range and the sources, then press **Start scan**.
4. Read the results in the app, or open `Report.txt` on your Desktop.

## Good to know

| Source | Needs | Note |
| --- | --- | --- |
| Deleted Prefetch / Recent | Administrator, NTFS | The journal has a limited size, so very old deletions may be overwritten |
| Security 4688 | Process creation auditing enabled | Empty if auditing was off |
| Sysmon | Sysmon installed | Empty if not installed |
| Prefetch / Recent | Prefetch needs Administrator | Timestamps are file times, not exact run times |

A keyword match is a hint, **not proof** of anything. Always look at the details before drawing conclusions.

Windows SmartScreen or your antivirus may warn about an unsigned app. Choose **More info > Run anyway** if you trust the download.

## Use responsibly

Only scan computers you own or have permission to check.

## License

[MIT](LICENSE)

---

## 🇮🇷 فارسی

یه برنامه ویندوزی که ردپای فعالیت‌های سیستم رو توی یه لیست قابل جستجو و یه فایل `Report.txt` جمع می‌کنه و **فایل‌های پاک‌شده‌ی Prefetch و Recent** رو هم نشون می‌ده.

**استفاده:** فایل exe رو از بخش [Releases](../../releases/latest) بگیر، اجراش کن و دسترسی Administrator رو تایید کن. بازه زمانی و منبع‌ها رو انتخاب کن و Start scan رو بزن.

**نکته:** پیدا شدن یه کلمه مشکوک به معنی اثبات چیزی نیست، فقط یه نشونه‌ست.
