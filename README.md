# alfresco-bart-docker
Dockerized version of [alfresco-backup-and-recovery-tool](https://github.com/toniblyx/alfresco-backup-and-recovery-tool), a backup and restore tool for Alfresco Document Store

## Usage
To run manually: 

``` docker run -e ALFBRT_PATH=/config -v=`pwd`/config:/config -v=`pwd`/backup:/mnt/backup -v=/opt/alfresco:/opt/alfresco -v=/var/run/postgresql:/var/run/postgresql -d sashman/alfresco-bart-docker```

By default this will display the BART help message.
