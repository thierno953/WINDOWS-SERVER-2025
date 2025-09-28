# BitLocker deployment (GPO + TPM+PIN + script)

📝SCRIPT

```sh
$pin=(Get-Random -Minimum 0 -Maximum 999999).ToString('000000')
echo "$pin" | out-file \\Srv25\PINS$\$env:computername.txt -Append
$SecureString = ConvertTo-SecureString "$pin" -AsPlainText -Force
Add-BitlockerKeyProtector -MountPoint "C:" -Pin $SecureString -TPMandPinProtector
msg * /time:0 Your hard drive is being encrypted. To start your PC, you need your Bitlocker-PIN, which is $pin
manage-bde -on c: -s -used -rp
schtasks /delete /tn BL /f
```

📋ARGUMENTS

```sh
-ExecutionPolicy Bypass -File \\Srv25\script$\BL.ps1
```