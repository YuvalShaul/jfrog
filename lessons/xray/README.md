


## Database

- Update DB Sync Daily Update Time.  
Based on [this link](https://www.jfrog.com/confluence/display/JFROG/Xray+REST+API#XrayRESTAPI-UpdateDBSyncDailyUpdateTime)  
**curl -u yuval:yuval http://artifactory.t5.devopsherpas.com/xray/api/v1/configuration/dbsync/time > -X PUT -d '{"db_sync_updates_time": "20:20"}' -H 'Content-Type: application/json'**
