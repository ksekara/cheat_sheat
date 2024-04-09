### find and remove files
``` linux
sudo find -name "*mongo*" -exec rm -r {} \;
```
### Transfer file
```
scp -i ~/.ssh/dev-server-usr1 /Downloads/blond_hair.jpg user1@123.231.95.165:
```

## Mount USB/external hard
```
mount /dev/sdb1 /media/external-hard/
```

### Copy files
```
sudo rsync -av /media/external-hard/<folder> /home/user1
```

### For error user1@123.231.95.165: Permission denied (publickey,gssapi-keyex,gssapi-with-mic)
```
check 
systemctl status sshd
if 
bad ownership
chmod go-w /home/user1
chmod 700 /home/user1/.ssh
chomd 600 /home/user1/.ssh/authorized_keys
```
https://chemicloud.com/kb/article/ssh-authentication-refused-bad-ownership-or-modes-for-directory/