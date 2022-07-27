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
