
# The jfrog cli

## CLI versions
- The current verion is cli v2.
- Both versions (v1, v2) are distributed, but updates will go to v2 only.
- See changes [here](https://www.jfrog.com/confluence/display/CLI/JFrog+CLI#JFrogCLI-ListofchangesinJFrogCLIv2)

## CLI Environment Variables

- CI  
If true, disables interactive prompts and progress bar.  
(default: false)
**export CI=true**
- Log level:  INFO/ERROR/DEBUG  
example:  
**export JFROG_CLI_LOG_LEVEL=DEBUG**
- More environment variables [here](https://www.jfrog.com/confluence/display/CLI/JFrog+CLI#JFrogCLI-EnvironmentVariables)

## Configure

- Download and install the cli - see [here](https://www.jfrog.com/confluence/display/CLI/JFrog+CLI#JFrogCLI-General).  
- Run the configuration:  
**jfrog  config add  <server ID>**
- Show:  
**jfrog config show  <server ID>**
- Remove:  
**jfrog config remove <server ID>**

## Files

- uoload a file:  
**jf rt u ./myfile.txt  generic-local/new/thefile**
- download a file:  
**jf rt dl  generic-local/new/thefile**
- Download multiple files:  
**jf rt dl  generic-local/new/\***

## Search

- To search files:
**jf rt s --spec=./search/spec1.txt**

## Copy/remove
- Copying files example:  
**jf rt cp generic-local/new/thefile  generic-local/new2/thefile**
- Moving file example:  
**jf rt mv generic-local/new/thefile2 generic-local/new2/thefile2**



## Creating builds:

- Basic creation of a build, with no info:  
**jfrog rt bp YuvBuild 1**
- For a detailed video see [here](https://www.youtube.com/watch?v=n9nAl4ofUfs)