#Install Module
Install-Module -Name PSWindowsUpdate -Force -AllowClobber

#Import Module
Import-Module PSWindowsUpdate

#Check updates
Get-WindowsUpdate

#Install KB
Get-WindowsUpdate -Install –KBArticleID <KB_number>

#Install all
Get-WindowsUpdate -AcceptAll -Install –AutoReboot

#History
Get-WUHistory

#Remove Specific Windows Updates
Remove-WindowsUpdate -KBArticleID KB5017308 –NoRestart

-------------------------------------------------------
#Hide KB
$HideList = “KB1234567” 
Get-WindowsUpdate -KBArticleID $HideList –Hide 

#Unhide
Show-WindowsUpdate -KBArticleID $HideList 
