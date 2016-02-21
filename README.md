# alfresco-bart-docker
Dockerized version of [alfresco-backup-and-recovery-tool](https://github.com/toniblyx/alfresco-backup-and-recovery-tool), a backup and restore tool for Alfresco Document Store

## Usage
To run manually: 

```docker run -e ALFBRT_PATH=/config -v=`pwd`/config:/config -it sashman/alfresco-bart-docker```

and then 

```/alfresco-backup-and-recovery-tool/src/alfresco-bart.sh backup```
