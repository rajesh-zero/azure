# azure
azure tips and tricks

taking windows terminal remote execute following in cloud shell
PS Azure:\> Enable-AzVMPSRemoting -Name rajesh -ResourceGroupName win
Azure:/
PS Azure:\> Enter-AzVM -name 'rajesh' -ResourceGroupName 'win' -Credential (get-credential)

where rajesh is name of vm and win is name of resource group

#downloading files from powershell
PS C:\Users\rajesh> [System.Net.ServicePointManager]::SecurityProtocol = 3072 -bor 768 -bor 192 -bor 48
PS C:\Users\rajesh> (New-Object Net.WebClient).DownloadFile('https://www.python.org/ftp/python/3.8.0/python-3.8.0.exe','python38.exe')
