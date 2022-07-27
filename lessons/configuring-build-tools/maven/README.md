# Maven Integration

Read about [maven repositories](https://github.com/YuvalShaul/jfrog/tree/master/lessons/configuring-build-tools/maven/maven-reps.md)
## Setting the repositor(ies) 

- Use the set-me-up button on the virtual maven
- Use encrypted password
- Create and download **settings.xml** into ~/.m2
- 

## Commands

- Install a package:  
**mvn install**  (will use seetings.xml in ~/.ms)  
    or
**mvn install -s settings.xml**   (specify your own settings file)
- Compile your package:  
mvn compile  

Demo in class:  
- Download from a remote central maven, by ..   
  - Remove slf4j from the local repo:  
    - cd ~/.m2/repository/org
    - rm -rf slf4j
  - Make sure it is also removed from the remote repository cache in artifactory
  - Compile:  
  **mvn clean compile**
  - Show cache in artifactory
- Deploy:  
**mvn deploy**


Maven if the oldest and most used in Artifactory.  

[todo] check about pom.xml settings.xml

[todo] check about package retreival and package publishing
setting that may change - get them out of the pom

[todo] try the "set me up" button.  
Will get you an XML file.  

What happens when you click the "download" button?

[todo] check about "cleanup Repository References in POMs"  
    
[todo] check about the "artifactory maven plugin"
- It can send build information to artifactory

