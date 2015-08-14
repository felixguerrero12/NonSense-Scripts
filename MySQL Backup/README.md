MySQL Backup Directions :

1. Place the cron script in the prefer cron job directory :

/etc/cron.monthly/ /etc/cron.weekly/  
/etc/cron.daily/  /etc/cron.hourly/

Depending on how often you want to do the back ups and what are the procedures in your enviroment.

2. Create the enviroment for the scripts to work :

a. mkdir /backup; mkdir /backup/scripts; mkdir /backup/mysqlbackups

NOTE : The /backup/scripts directory is where all the mysql script should be located. The /backup/mysqlbackups is where all the mysql backups will be stored.

3. Place them MySQL Backup script in the /backup/scripts directory :
a. Create the MySQL backup script file :
    I. cd /backup/scripts
    II. vi mysqlbackup-localhost
    Copy the script; Press i; Paste the script; Press Escape; Enter x;

Note : Before you create the MySQL backup script make sure you add root password in the <password> section part of the script.
