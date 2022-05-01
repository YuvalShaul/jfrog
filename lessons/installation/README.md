
## JFROG Directories

- The **$JFROG_HOME** points to the main directory of the installation.  
In some cases (RPM/Debian) this is:  
**/opt/jfrog**  
We can create the JFROG_HOME env var to point there (not done by default).
- The **Application** directory is at:  
**JFROG_HOME/<product>/app**
- The **Data** directory is at:  
**JFROG_HOME/<product>/var**  
(this is actually a logical link)
- Regarding the /opt directory:  
According to the Filesystem Hierarchy Standard, /opt is for “the installation of add-on application software packages”.

- System Smoke Test:  
**curl -u yuval:yuval http://artifactory.t5.devopsherpas.com/artifactory/api/system**
- 