# passCreate
Create an encrypted Password using Tetaterm macro, and save it in .dat file

# 1st point
# Create batch server user password for sysg and root
# Fix hostname and add the target servers if you need
BT01sysg = 'hostname-sysg'
BT01root = 'hostname-root'

# 2nd point
# save password in passwd.dat
PWFile = 'passwd.dat'

# 3rd point
# When initial connection, the pop-up is displayed, and write the password
# Depending on 1st point, add the target servers
getpassword PWFile BT01sysg loginPW
getpassword PWFile BT01root switchPW

end
