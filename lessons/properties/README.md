

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
- Setting some properties on a directory using matrix parameters:  
**curl -X PUT -uyuval:'Yuval123#'  'http://artifactory.t5.devopsherpas.com/artifactory/api/storage/maven-dev-local/com?properties=os=win,linux;qa=done&recursive=1'**
- Deploy a file with properties:  
**curl -T file.txt -uyuval:'Yuval123#'  'http://artifactory.t5.devopsherpas.com/artifactory/generic-local/myfile.txt;prop1=val1;prop2=val2'**







- demonstrate with the browser:
  - http://artifactory.t5.devopsherpas.com/ui/native/maven-prop
  - 

http://artifactory.t5.devopsherpas.com/artifactory/maven-dev-local/org


curl -u yuval:Yuval123# http://artifactory.t5.devopsherpas.com/artifactory/api/search/prop?thename:yuval  