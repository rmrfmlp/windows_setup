`winget import -i packages.json --accept-package-agreements --accept-source-agreements`

If hash errors:
```
winget source reset --force
winget source update
```

Then re-run
