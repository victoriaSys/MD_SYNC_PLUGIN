SysbindApi For Moodle
=============================

Configuration
-------------
1. This plugin requires `webservice_restful` plugin. 
Notice: the version that was devloped by Frédéric Massart <fred@branchup.tech>.
2. Checkout to MOODLE_401_SYSBIND branch
3. Should be enabled:
   - `web services`
   - `protocols: rest,restful`
  

Usage
-----
On Administration > Local Plugins > Sysbind REST API Service > Mapping > Add a mapping:
1. Choose a service you want to map
2. Choose a webservice username
3. Define all the required fields with relevant names
4. Select a keyfield (Username is recommended for users service, Idnumber for the other services)
5. Save changes - This will automatically create a token for this webservice username
   
You should create all the services: users, courses, categories, groups and enrolls.
Check the documentation of the possible requests for each service.


Notice
------
* Make sure you allow role assignment for the SysbindApi role for the following roles: "students","teacher","non-editing teacher"
on Administration > Users > Allow role assignment



Author
------
SysBind LTD.
