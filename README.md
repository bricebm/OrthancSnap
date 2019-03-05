# OrthancSnap

Orthanc.json lives in /var/snap/orthanc/current/config-files

Defautl storage is in /var/snap/orthanc/current/

1. Services managed by snap:
    * sudo snap services orthanc -- will show current status
    * sudo snap restart|stop|start orthanc
    * sudo snap stop --disable|enable orthanc
    * sudo snap logs orthanc -f

2. If you want to build locally
    * Install snapcraft
        ```$ sudo snap install snapcraft --classic```
    * Install multipass
        ```snap install multipass --beta --classic```
    * Clone the repo
    * Run snapcraft command from within the directory
        ```snapcraft```
    * This will produce an snap package that can be installed locally
        ```sudo snap install <orthanc-snap> --dangerous```
        * --dangerous flag is needed due to sideloading the snap package.
    * Snapcraft documentation can be found at snapcraft.io

