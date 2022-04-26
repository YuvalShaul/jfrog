# Artifactory REST APIs

## Using curl

Here are some uses of curl tool:  
- Simple use (uses GET by default):  
**curl 


## Authentication



## Demos (user/password authentication)

- A **ping** ([doc](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-SystemHealthPing)):  
**curl -u yuval:yuval  http://artifactory.t5.devopsherpas.com/artifactory/api/system/ping**
- Complete system info ([doc](https://www.jfrog.com/confluence/display/JFROG/Artifactory+REST+API#ArtifactoryRESTAPI-SystemInfo)):  
**curl -u yuval:yuval http://artifactory.t5.devopsherpas.com/artifactory/api/system**