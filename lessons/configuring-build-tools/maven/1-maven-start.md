## Maven installation

- Make sure maven is installed:  
**mvn --version**
- If it is not installed, use [this link](https://maven.apache.org/guides/getting-started/maven-in-five-minutes.html) to see installation instructions.
- In the result you can see the maven installation directory (**/usr/share/maven** in my Ubuntu).


## Maven project

- To create a project, type the following command:  
**mvn archetype:generate -DgroupId=com.mycompany.app -DartifactId=my-app -DarchetypeArtifactId=maven-archetype-quickstart -DarchetypeVersion=1.4 -DinteractiveMode=false**
- The command has created a directory with the same name of the artifactId.  
CD into the directory:  
**cd my-app**
- Here is the standard project structure:  
```
my-app  
|-- pom.xml  
`-- src  
    |-- main  
    |   `-- java  
    |       `-- com  
    |           `-- mycompany  
    |               `-- app  
    |                   `-- App.java  
    `-- test  
        `-- java  
            `-- com  
                `-- mycompany  
                    `-- app  
                        `-- AppTest.java  
```


