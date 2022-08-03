Explain:
- A Docker repository is where you can store 1 or more versions of a specific Docker image. 
- An image can have 1 or more versions (tags).
- **a jfrog docker repository is actually called a registry in docker.**


- docker login <repository>
- To host multiple registries (single artifactory host),  
docker will have to convert:  
```
     docker pull <art host>/<repository>:<docker tag>  
        to  
     docker build <repository>.<art host>/:<docker tag>  
```
  - port mapping: a port mapped to a each repository (i.e: registry)
