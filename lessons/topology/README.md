# Topology

## Federated Repositories

- Create a federated repositories in  HOME, called **fed6**
- Choose "federated" tab to make sure another one is created in Europe
- Upload a jar file into HOME repo:  
**jfrog rt u postgresql-42.3.4.jar fed6**
- Make sure it was also created in Europe
- Delete, and see that it was deleted.


## Push Replications

- Choose repository **maven-dev-local**
- Configure replication:
  - Cron:   0 0 12 * * ?
  - Check **Enable Event Replication**
  - URL:  http://europe.t5.devopsherpas.com/artifactory/maven-dev-main
  - User/Pass yuval yuval
  - Test should pass
- Upload a file:  
**jfrog rt u postgresql-42.3.4.jar maven-dev-local**


## Pull Replication

- Choose **rem-maven-b** from Europe
- It is a remote configured to point to team1-maven-dev-local
- URL:  
**http://artifactory.t5.devopsherpas.com/artifactory/team1-maven-dev-local**
- In the replication DO NOT FILL URL.  
Only enable it - it know where to look.
- Upload file to local in HOME:  
**jfrog rt u postgresql-42.3.4.jar team1-maven-dev-local**