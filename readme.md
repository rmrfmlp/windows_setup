Quick installer to install the following into Windows. This replaces Ninite like functionality.
Ideally Windows has been installed with an unattend.xml file that decrapifies it (https://schneegans.de/windows/unattend-generator/)

Run `winget import -i <JSON_FILE_HERE> --accept-package-agreements --accept-source-agreements`

If hash errors:
```
winget source reset --force
winget source update
```

Then re-run

Install Files.Community using Powershell (hash isn't matching on WinGet so not installing currently):  
`Add-AppxPackage -AppInstallerFile https://cdn.files.community/files/stable/Files.Package.appinstaller`
