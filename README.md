A mongo container with periodic backups.

## Environment Variables

* `HOST` (default: localhost) : the hostname of the mongodb server to backup
* `PREFIX` (default: mongodb) : the prefix part of the backup archive filename. The name will
  also include a date-time field.
* `INTERVAL` (default: 86400) : the number of seconds between each backup that will be taken.
  If set to zero, then the container will run the process once and exit.

## Volumes

* `/backups` : this where the script will place the backup archives by default
