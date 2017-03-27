# mysqlBackup
Backup script for a remote Mysql/MariaDB server. Stores each database in a separate directory with a single md5 file for verification.

### Example
mysqlBackup -d /var/backup/mydb/ -h 192.168.0.1 -u admin -p mypassword

### Return codes
0) Successfull backup
1) Missing parameter
2) Directory does not exist or is not writable.
3) mysqldump is missing or can not be found in path.
4) backup directory could not be created
