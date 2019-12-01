# azure
azure tips and tricks

taking windows terminal remote execute following in cloud shell
PS Azure:\> Enable-AzVMPSRemoting -Name rajesh -ResourceGroupName win
Azure:/
PS Azure:\> Enter-AzVM -name 'rajesh' -ResourceGroupName 'win' -Credential (get-credential)
