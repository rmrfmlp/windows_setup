Quick installer to install the following into Windows. This replaces Ninite like functionality.
Ideally Windows has been installed with an unattend.xml file that decrapifies it (https://schneegans.de/windows/unattend-generator/)

```
        { "PackageIdentifier": "Google.Chrome" },
        { "PackageIdentifier": "Mozilla.Firefox" },
        { "PackageIdentifier": "Waterfox.Waterfox" },
        { "PackageIdentifier": "dotPDN.PaintDotNet" },
        { "PackageIdentifier": "Zoom.Zoom" },
        { "PackageIdentifier": "SublimeHQ.SublimeText.4" },
        { "PackageIdentifier": "Notepad++.Notepad++" },
        { "PackageIdentifier": "VideoLAN.VLC" },
        { "PackageIdentifier": "WinDirStat.WinDirStat" },
        { "PackageIdentifier": "7zip.7zip" },
        { "PackageIdentifier": "File-New-Project.EarTrumpet" },
        { "PackageIdentifier": "Mozilla.Thunderbird" },
        { "PackageIdentifier": "OBSProject.OBSStudio" },
        { "PackageIdentifier": "Google.ChromeRemoteDesktopHost" },
        { "PackageIdentifier": "voidtools.Everything" },
        { "PackageIdentifier": "FilesCommunity.Files" },
        { "PackageIdentifier": "QL-Win.QuickLook" }
```

Run `winget import -i packages.json --accept-package-agreements --accept-source-agreements`

If hash errors:
```
winget source reset --force
winget source update
```

Then re-run
