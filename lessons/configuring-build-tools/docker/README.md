[todo]
- v1 and v2 - but most use v2
- docker login <repository>
- To host multiple registries (single artifactory host):
  - repository path: 
     docker pull \<art host\>/\<repository\>:\<docker tag\>  
  - subdomain (recommended)  
docker build \<rep name\>.artifactory...
  - port mapping: a port mapped to a repository
- Configure in Helm?
- If it is insecure - add to insecure
- Docker have limited access to dockerhub, so a remote rep solves that
command:
- docker login
- docker push
- docker pull
