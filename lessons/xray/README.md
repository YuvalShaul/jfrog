

## XRay Architecture

**https://www.jfrog.com/confluence/display/JFROG/Xray+Security+and+Compliance**

## IDE integration

**https://www.jfrog.com/confluence/display/JFROG/IDE+Integration**

## Installation
Installation:
  **https://www.jfrog.com/confluence/display/JFROG/Installing+Xray**
Master key
  **/opt/jfrog/xray/var/etc/security/master.key**

## Database

- Get DB update time:  
**curl -u yuval:yuval http://artifactory.t5.devopsherpas.com/xray/api/v1/configuration/dbsync/time**
- Update DB Sync Daily Update Time.  
Based on [this link](https://www.jfrog.com/confluence/display/JFROG/Xray+REST+API#XrayRESTAPI-UpdateDBSyncDailyUpdateTime)  
**curl -u yuval:yuval http://artifactory.t5.devopsherpas.com/xray/api/v1/configuration/dbsync/time > -X PUT -d '{"db_sync_updates_time": "20:20"}' -H 'Content-Type: application/json'**
