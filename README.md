# Installation

```powershell
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser -Force
iex "& {$(irm https://gitea.com/magicedy/scoop-bucket-m/raw/branch/master/install.ps1)} -ScoopDir c:\scoop"
# For Admin
# iex "& {$(irm https://gitea.com/magicedy/scoop-bucket-m/raw/branch/master/install.ps1)} -ScoopDir c:\scoop -RunAsAdmin"
scoop install aria2 git
scoop bucket rm main
scoop bucket add main https://gitea.com/magicedy/scoop-bucket-m
```
