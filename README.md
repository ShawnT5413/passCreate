## passCreate
### Create an encrypted Password using Tetaterm macro, and save it in .dat file

Create batch server user password for sysg and root
Fix hostname and add the target servers if you need
```
BT01sysg = 'hostname-sysg'
BT01root = 'hostname-root'
```

Save password in passwd.dat
```
PWFile = 'passwd.dat'
```

When initial connection, the pop-up is displayed, and write the password
Depending on fixing servers, add the target servers
```
getpassword PWFile BT01sysg loginPW
getpassword PWFile BT01root switchPW
```
