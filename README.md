# alfresco-bart-docker
Dockerized version of [alfresco-backup-and-recovery-tool](https://github.com/toniblyx/alfresco-backup-and-recovery-tool), a backup and restore tool for Alfresco Document Store

## Usage
To run manually: 

``` docker run -e ALFBRT_PATH=/config -v=`pwd`/config:/config -v=`pwd`/backup:/mnt/backup -v=/opt/alfresco:/opt/alfresco -v=/var/run/postgresql:/var/run/postgresql sashman/alfresco-bart-docker```

By default this will display the BART help message. To perform a back up, append `backup` argument to the above command.

### Parameters

* ```-e ALFBRT_PATH=/config -v=`pwd`/config:/config``` - Provide the directory for the config files, and set it as env variable.
* ```-v=`pwd`/backup:/mnt/backup``` - Provide the destination directory if performing a local backup.
* ```-v=/opt/alfresco:/opt/alfresco``` - Alfresco directory to backup.
* ```-v=/var/run/postgresql:/var/run/postgresql``` - Optional for usage of postgres socket connections.
