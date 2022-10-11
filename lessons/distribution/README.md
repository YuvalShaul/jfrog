# Distribution

## Keys

- [GPG Signing](https://www.jfrog.com/confluence/display/JFROG/GPG+Signing)  
(including multiple keys)


## Create a Release Bundle

- We have a maven application inside maven-dev-local repository
- Specify the repository name in the repository build
- Specify:  
**maven-dev-local/mycompany/app/\***  
in the **include artifact path patterns**


## Smart Remote Repositories

- Create a remote docker repository in Asia
- Use this to point to docker-dev-local (in US):  
**http://artifactory.t5.devopsherpas.com/artifactory/docker-dev-local**
