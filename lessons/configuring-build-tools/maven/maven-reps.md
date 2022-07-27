# Maven repositories

## Repositories Structure

In Maven terminology, a repository is a directory where all the project jars, library jar, plugins or any other project specific artifacts are stored and can be used by Maven easily.

Maven repository are of three types. The following illustration will give an idea regarding these three types.

    local
    central
    remote
![maven repositories structure](https://user-images.githubusercontent.com/40225170/181215676-bf28c57a-f024-4aa2-aa1f-b34cb2523055.jpg)


## Local Repository

Maven local repository is a folder location on your machine. It gets created when you run any maven command for the first time.

Maven local repository keeps your project's all dependencies (library jars, plugin jars etc.). When you run a Maven build, then Maven automatically downloads all the dependency jars into the local repository. It helps to avoid references to dependencies stored on remote machine every time a project is build.

Maven local repository by default get created by Maven in %USER_HOME% directory.   
On my linux I could find the local repository at:   
**~/.m2**


## Central Repository

Maven central repository is repository provided by Maven community. It contains a large number of commonly used libraries.

When Maven does not find any dependency in local repository, it starts searching in central repository using following URL − https://repo1.maven.org/maven2/

Key concepts of Central repository are as follows −

    This repository is managed by Maven community.
    It is not required to be configured.
    It requires internet access to be searched.

To browse the content of central maven repository, maven community has provided a URL − https://search.maven.org/#browse. Using this library, a developer can search all the available libraries in central repository.