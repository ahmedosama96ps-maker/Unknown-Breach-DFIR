# Artifact Summary

| Artifact / Area | Tool | Finding | Interpretation |
|---|---|---|---|
| Operating system and users | Autopsy / file system | Windows environment with multiple user profiles | Established the investigation context and users of interest |
| Recent documents / LNK | Autopsy | References to `New Prices`, `NewPrices.txt`, and related pricing files | Supported user interaction with pricing-related data |
| Recycle Bin | Autopsy | Deleted `New Prices` folder, `.mdb` database, and text files | Supported deleted-file / cleanup activity |
| Browser / keyword artifacts | Autopsy | References to “How to Hide Money From the Government” | Relevant to the financial-concealment hypothesis |
| USB artifacts | Autopsy | Lexar JumpDrive, SanDisk Card Reader, Kingston DataTraveler | Confirmed removable-media usage; file transfer itself was not proven |
| Run / RunOnce | Registry Explorer | No suspicious entries | No suspicious user-logon persistence through these keys |
| UserAssist | Registry Explorer | Mostly normal applications | No clearly suspicious program execution identified from UserAssist |
| Prefetch | Autopsy / Velociraptor | Standard Windows processes, including `RUNDLL32.EXE` | No clear malicious execution trace from available Prefetch |
| ShimCache / AppCompatCache | Registry Explorer | `BCTextEncoder.exe` under Jimmy Wilson's Desktop | Strong artifact linking the encoding tool to the user profile |
| Amcache | File-system analysis | `Amcache.hve` not present | Limited executable metadata analysis through Amcache |
| IOC search | Velociraptor | Located `G:\USERS\Jimmy Wilson\Desktop\BCTextEncoder.exe` | Corroborated the suspicious encoding-tool finding |
| Startup folder persistence | Velociraptor | Only `desktop.ini` identified | No suspicious Startup-folder persistence found |
