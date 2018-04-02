## Useful snippets

### MySQL
Backup and restore 
```
mysqldump -u *username* -p *database_name* > *output.file*
mysql -u *username* -p --port=XXXX *database_name* < *output.file*
```

### MongoDB
Start service, check status and add to system start (creates symlink from /etc/systemd/system/multi-user.target.wants/mongod.service to /lib/systemd/system/mongod.service)
```
sudo systemctl start mongod
sudo systemctl status mongod
sudo systemctl enable mongod
```
