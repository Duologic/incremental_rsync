incremental_rsync
=================


This script can make incremental backups with Rsync.
- from local to local
- from local to remote
- from remote to local

Todo: 
- from remote to remote

Execute as:

    ./incremental_rsync /path/to/config.cfg

Config file:

    prefix="my_backup"
    source_ssh="false"
    source="/home"
    #source_key=""
    #source_user=""
    #source_host=""
    
    destination_ssh="true"
    destination="/backup"
    destination_key="/home/user/.ssh/rsync-key"
    destination_user="root"
    destination_host="backup.somedomain.tld"
    
    from_mail="noreply@somedomain.tld"
    to_mail="admin@somedomain.tld"
    smtp_server="smtp.somedomain.tld"

