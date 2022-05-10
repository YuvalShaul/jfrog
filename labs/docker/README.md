

## Prepare

- Create a local docker repository (**docker-dev-local**)
- Create a remote docker repository (**docker-remote**)
- Create a virtual docker repository.
  - Add the local and the remote repositories to the virtual repository.
  - Configure the local repository as the default deployment repository
- Add the new virtual repository to your **/etc/hosts** file.  
Example:  
**34.238.65.31 artifactory.t5.devopsherpas.com  docker-virtual.artifactory.t5.devopsherpas.com**
- Make sure your HTTP Settings are correct:  
Administration/Artifactory/HTTP settings:  
  - Access Method:  Sub Domain  
  - Serer Provider: NGINX
  - public: artifactory.t5.devopsherpas.com
  - HTTP port: 80
  - No HTTPS
- Add new name to insecure-registries in docker configuration: (since you're not going to use https)
/etc/docker/daemon.json :  
  {  
  "insecure-registries" : ["virtual-docker.artifactory.t5.devopsherpas.com"]  
  }  
- Restart docker so that it will take effect:  
**systemctl restart docker**

## Login to your virtual docker repository

- **docker login docker-virtual.artifactory.t5.devopsherpas.com**  
(use your admin:password you use to login to artifactory)


## Do some docker stuff

- Make sure your remote repository cache has no image in it
- Pull some image from your virtual rep:  
**docker pull docker-virtual.artifactory.t5.devopsherpas.com/busybox:latest**  
(it should take some time untill you see that image in the remote cache)
- Push this image:  
**docker push docker-virtual.artifactory.t5.devopsherpas.com/busybox:latest**
