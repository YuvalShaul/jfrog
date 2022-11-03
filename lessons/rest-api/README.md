# Artifactory REST APIs

## Using curl

Here are some uses of curl tool:  
- Simple use (uses GET by default):  
**curl 


## Authentication



## Demos (user/password authentication)

- A **ping** ([doc](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-SystemHealthPing)):  
**curl -u yuval:'Yuval123#'  http://artifactory.t5.devopsherpas.com/artifactory/api/system/ping**
- Complete system info ([doc](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-SystemInfo)):  
**curl -u yuval:'Yuval123#' http://artifactory.t5.devopsherpas.com/artifactory/api/system**
- Download a file:  
**curl  -uyuval:'Yuval123#' "http://artifactory.t5.devopsherpas.com/artifactory/generic-local/myfile.txt"**

- Upload a file into a new directory:  
**curl -u yuval:'Yuval123#' -X PUT "http://artifactory.t5.devopsherpas.com/artifactory/maven-prop/newdiry/file.txt" -T file.txt**
