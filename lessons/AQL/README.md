
The notion of a domain:
- item
- ..

Run the cli search in debug mode to see

## Examples

- Contents of a repo:  
**curl -u yuval:yuval -X POST http://artifactory.t5.devopsherpas.com/artifactory/api/search/aql -H 'Content-Type: text/plain' -d 'items.find({"repo":"docker-dev-local"})'**
- Based on a file query:  
**curl -u yuval:yuval -X POST http://artifactory.t5.devopsherpas.com/artifactory/api/search/aql -T q.txt**
