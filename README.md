# Postgres pg_dump backup

Perform a pg_dump database backup, attach current_data to name and coppy to specified backup_server/s3 endpoint. S3 or backup_server needs to be defined

## Requirements

## Variables

|Variable Name|Default Value|Required|Description|Example|
|:---|:---:|:---:|:---|:---|
|`backup_directory`|"/var/lib/backups"|no|Temporary directory to store the created backup files|'/opt/backups'|
|`backup_server`| - |no|Speficy a backup server - take a look at the default example| - |
|`databases`| - |yes|A list of exiting databases to backup| - |
