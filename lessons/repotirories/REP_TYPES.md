

## Local Repository


## Remote Repository

- A remote repository is a ["a proxy for a repository located on a remote server."](https://jfrog.com/knowledge-base/what-is-a-remote-repository-and-how-does-it-work/)
- As it's typically configured:
  - Artifactory will look in the local cache of your remote repository
    - If the file is not in the local cache, then Artifactory will go to the internet to attempt to obtain the resource
    - If the resource is finally located, Artifactory will cache it locally and serve it to the client
- [A remote repository never pre-fetch a resource](https://www.jfrog.com/confluence/display/JFROG/Repository+Management)


## Virtual Repository

- A virtual rep. is not a remote rep.
- It aggregates several repositories with the same package type under a common URL
- These can be local, remote, and also virtual.
- There CAN be [Generic Virtual Repositories](https://www.jfrog.com/confluence/display/JFROG/Repository+Management).  
By their nature, Virtual Repositories whose package type has been specified as Generic can aggregate repositories of any type, however generic virtual repositories do not maintain any metadata.
- Virtual repository seach (resolution) order:
  - Order of repository types:
    - **local**
    - **remote  repository caches**
    - **remote repositories themselves**
  - Order within a single repository type:
    - the order in which they are listed in the configuration
  - For a virtual repository, you can see the effective search and resolution order in the Included Repositories list view in the Basic settings tab.