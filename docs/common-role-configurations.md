---
sidebar_label: 'Common Role Configurations'
hide_title: 'true'
---

# Common Role Configurations

### Best Practices

* Three main user Groups (Roles) For OpCon Privileges:  
    * **Administrators**
    * **Schedulers**
    * **Operators**

#### Administrators

* OpCon Administrator(s) must ensure all OpCon Users have needed Privileges 
* The OpCon Administrator with the User ID ```ocadm``` is automatically granted all Privileges to everything within OpCon, **including** access to ‘Server Options’ and the ability to edit Schedule or Job Frequencies affecting multiple Jobs
* When creating new Administrator User accounts, desired Privileges must be purposefully selected

#### Schedulers

* These individuals will build and maintain Jobs and Schedules 
* They will need as much access as possible to every section within Enterprise Manager except for ‘Administration’ section 
* Privileges listed in chart can be used as a guide for assigning Privileges to OpCon Schedulers

![](../static/img/316-64377c7303aecb43e324bd34323ad13b.png)

![](../static/img/commonconfigs.png)

#### Operators

* These individuals will monitor Jobs and Schedules on daily basis 
* They will need authority to see every Schedule and be able to perform maintenance before and after a Job and/or Schedule runs (Restart Jobs, Force-Start Jobs, Force-Start Schedules, Release Schedules, etc.) 
* Privileges listed in the chart can be used as a guide for assigning Privileges to OpCon Operators

![](../static/img/318-fa792342afe6f0eaf5ecb20c5ff60c38.png)

![](../static/img/commonconfigs2.png)