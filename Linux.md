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