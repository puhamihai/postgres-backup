# Postgres pg_dump backup

Perform a pg_dump database backup, append current_data(now(fmt='%Y-%m-%d_%H-%M-%S')) to the backup name, and copy the resulting file the to specified backup_server or S3 endpoint.

NOTE: For Debian fammily servers, make sure the acl package is installed!
```bash
sudo apt-get install acl
```
## Requirements

## Variables

|Variable Name|Default Value|Required|Description|Example|
|:---|:---:|:---:|:---|:---|
|`backup_directory`|"/var/lib/backups"|no|Temporary directory to store the created backup files|'/opt/backups'|
|`backup_server`| - |no|Speficy a backup server - take a look at the default example| - |
|`databases`| - |yes|A list of exiting databases to backup| - |
