# Maven Integration

## Maven repositories

In Maven terminology, a repository is a directory where all the project jars, library jar, plugins or any other project specific artifacts are stored and can be used by Maven easily.

Maven repository are of three types. The following illustration will give an idea regarding these three types.

    local
    central
    remote
![maven repositories structure](https://user-images.githubusercontent.com/40225170/181215676-bf28c57a-f024-4aa2-aa1f-b34cb2523055.jpg)

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

