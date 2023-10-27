# Installation

```powershell
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser -Force
iex "& {$(irm https://codeberg.org/magicedy/scoop-bucket-m/raw/branch/master/install.ps1)} -ScoopDir c:\scoop"
# For Admin
# iex "& {$(irm https://codeberg.org/magicedy/scoop-bucket-m/raw/branch/master/install.ps1)} -ScoopDir c:\scoop -RunAsAdmin"
scoop install git
scoop config SCOOP_REPO https://codeberg.org/magicedy/Scoop
scoop bucket rm main
scoop bucket add main https://codeberg.org/magicedy/scoop-bucket-m

scoop config global_path c:\scoop_global
```
