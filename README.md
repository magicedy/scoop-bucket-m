# Installation

```powershell
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser -Force
iex "& {$(irm https://gitea.com/magicedy/scoop-bucket-m/raw/branch/master/install.ps1)} -ScoopDir c:\scoop"
# For Admin
# iex "& {$(irm https://gitea.com/magicedy/scoop-bucket-m/raw/branch/master/install.ps1)} -ScoopDir c:\scoop -RunAsAdmin"
scoop install git
scoop config SCOOP_REPO https://gitea.com/magicedy/Scoop
scoop bucket rm main
scoop bucket add main https://gitea.com/magicedy/scoop-bucket-m

scoop config global_path c:\scoop_global
```
