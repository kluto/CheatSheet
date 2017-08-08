## Useful PostreSQL and MySQL snippets

# MySQL
Backup and restore 
mysqldump -u *username* -p *database_name* > *output.file*
mysql -u *username* -p --port=XXXX *database_name* < *output.file*
