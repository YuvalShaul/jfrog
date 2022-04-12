

- A lot of artifacts
- We need metadata or properties
- Searching for artifacts based on metadata
- Benefits:
  - where is it deployed
  - trace binary to its origin
  - pick the right one for production
- Can attach it to both file and folders (demo)
- a property-set - a set of properties - actually just in UI


Adding metadata:
- custom properties (yourself)
- implicit (automatically by artifactory)

Consuming metadata:
- Using AQL
- 

Setting:
- Artifacts
- directories (recursivley)
- using property-set

Retreive:
- Using a URL:
  - Non-conflicting (even if the property is not there - artifact will be returned)
  - mandatory (only if the property is there and the same value - using a plus sign)
- Multiple values (this is a logical AND)
- 


