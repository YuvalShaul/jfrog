

## Repository with 4 items
- Create a local repository called **maven-prop**
- download from maven central and upload into the repository:
  - **jfrog rt u images-1.0.0.jar maven-prop**
  - **jfrog rt u math-2022.14.jar maven-prop**
  - **jfrog rt u gui-1.1.1.jar maven-prop**
  - **jfrog rt u db-1.0.2.jar maven-prop**
- Assign **prop1** property with values 1, 2, 3, 4 to those artifacts.



## Matrix Parameters

- Get them:  
**curl -u "yuval:Yuval123#" "http://artifactory.t5.devopsherpas.com/artifactory/api/search/prop?prop1=1"**  
**curl -u yuval:Yuval123# "http://artifactory.t5.devopsherpas.com/artifactory/api/search/prop?prop1=2"**  
**curl -u yuval:Yuval123# "http://artifactory.t5.devopsherpas.com/artifactory/api/search/prop?prop1=3"**  
**curl -u yuval:Yuval123# "http://artifactory.t5.devopsherpas.com/artifactory/api/search/prop?prop1=4"**  


http://artifactory.t5.devopsherpas.com/artifactory/maven-dev-local/org


curl -u yuval:Yuval123# http://artifactory.t5.devopsherpas.com/artifactory/api/search/prop?thename:yuval  