ENUMERATING EVERTHING

```bash
enum4linux-ng IP
```

CONNECTING TO SMB SERVER AND LISTING THE SHARES

```bash
smbclient -L IP
```

CONNECTING TO A SHARE

```bash
smbcleint //IP/SHARE_NAME
```

### NETEXEC

LISTING ALL THE USERS WITHOUT CREDS

```bash
netexec smb IP -u '.' -p '' --rid-brute
```

LISTING ALL THE USERS WITH CREDS

```bash
netexec smb IP -u 'user' -p 'password' --users
```

LISTING ALL THE SHARES

```bash
netexec smb IP -u 'user' -p 'password' --shares
```

LISTING ALL GROUPS

```bash
netexec smb IP -u 'user' -p 'password' --groups
```

GETTING ALL THE LOGGEDON USERS

```bash
netexec smb IP -u 'user' -p 'password' --loggedon-users
```

SPIDERING A SHARE

```bash
netexec smb IP -u 'user' -p 'password' -M spider_plus --share 'SHARE_NAME'
```

GETTING THE PASSWORD POLICY

```bash
crackmapexec smb IP -u user -p Password123 --pass-pol
```

### USING RPCCLIENT

```bash
rpcclient -U "" -N IP

getdominfo-getting domain info
getdompwinfo- getting domain password info
getdomuser-getting the domian users
srvinfo-server information
```

### USING SMBMAP

CHECKING HOST

```bash
smbmap -H IP
```

LISTING ALL THE DIRECTORY OF A SHARE

```bash
smbmap -u 'user' -p 'password' -d domain.local -H IP -R 'SHARE_NAME' --dir-only
```
