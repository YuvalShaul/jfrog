
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
**jfrog  config**
- 

## Profile examples

- show  
jfrog config show
- add  
jfrog config add
- remove  
jfrog config remove

## Files

- download  
jfrog rt download \<file\>


## Creating builds:

- Basic creation of a build, with no info:  
**jfrog rt bp YuvBuild 1**
- For a detailed video see [here](https://www.youtube.com/watch?v=n9nAl4ofUfs)