# Artifactory Build Integration



## Links

- Build info:  
https://buildinfo.org/

## Demo

- Upload a first file:  
**jfrog rt u postgresql-42.3.4.jar maven-stage-local --server-id=yuvcfg  --build-name=demo --build-number=1**
- Download a second file (same build name, same build number):  
**jfrog rt dl  maven-stage-local/repomd.xml --server-id=yuvcfg  --build-name=demo --build-number=1**
- Now publish the build (**bp** means build-publish):  
**jfrog rt bp demo 1 --server-id=yuvcfg**

