# SMB Enumeration

## Using Enum4linix/Enum4linux-ng

`enum4linux-ng IP`

## Using Smbclient

`smbclient -L IP`

`smbcleint //IP/SHARE_NAME`

## Using Smbmap

`smbmap -H IP`

`smbmap -u user -p password -d doamain.local -H IP -R 'SHARE_NAME' --dir-only `


## Using crackmapexec

`crackmapexec smb IP -u 'user' -p 'pass' --shares`

`crackmapexec smb IP -u 'user' -p 'pass' --users`

`crackmapexec smb IP -u 'user' -p 'pass' --groups`

`crackmapexec smb IP -u 'user' -p 'pass' --loggedon-users`

`crackmapexec smb IP -u 'user' -p 'pass' -M spider_plus --share 'Share_name' `

## Using rpcclient

`rpcclient -U "" -N 172.16.5.5` 

