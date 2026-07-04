# Safe Delete

Goal:
Help users recover storage without damaging Windows or installed software.

Always classify items as:

🟢 Safe
- Temp folders
- Browser cache
- Windows Update cache
- Build outputs
- npm cache
- pip cache
- conda cache

🟡 Review
- Downloads
- ISO files
- Old VM images
- Duplicate folders

🔴 Never delete automatically
- Windows
- Program Files
- ProgramData
- EFI
- Recovery
- pagefile.sys
- hiberfil.sys
- Active project folders

Always ask for confirmation before deleting anything larger than 1 GB.
