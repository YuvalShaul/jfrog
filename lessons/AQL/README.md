
The notion of a domain:
- item
- ..

Run the cli search in debug mode to see

## Examples

- Contents of a repo:  
**curl -u yuval:yuval -X POST http://artifactory.t5.devopsherpas.com/artifactory/api/search/aql -H 'Content-Type: text/plain' -d 'items.find({"repo":"docker-dev-local"})'**
- Based on a file query:  
**curl -u yuval:yuval -X POST http://artifactory.t5.devopsherpas.com/artifactory/api/search/aql -T q.txt**
- Setting some properties on a directory using the matrix parameters:  
curl -H 'X-JFrog-Art-Api: AKCp8mYUmekG3L6jqHnNKw45NiSp1W42pLRYum9rZ25zq5brigKLcX9bR5up2s2yXnZp6KgP2' –X PUT 
"http://artifactory.t5.devopsherpas.com/artifactory/api/storage/artifactory.t5.devopsherpas.com/busybox? properties=os=win,linux;qa=done&recursive=1"
