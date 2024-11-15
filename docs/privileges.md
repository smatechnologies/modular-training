---
sidebar_label: 'Privileges'
hide_title: 'true'
---

# Privileges

### Privileges

* The Administrator can grant a variety of Privileges to Roles using the Role Definition sections on the Role page:
  * General
  * Activities
  * Batch Users
  * Departments
  * Resources

![](../static/img/Privileges-3d96bfb55e975a93d3f6cdf49f9adc01.png)

* Machines and Machine Groups are maintained using the **Agents** table.
* Access Codes, Batch Users, and Departments are created on corresponding screens within **Security** section of the **Library**

![](../static/img/SecuritySection-f6a6fbe5d02ca92b8820f478a8bd6ab1.png)

### Machine Privileges

* Machine Privileges are used to control Machines for Users in a Role that have Privileges to create and edit Jobs
* Within Master Job and Operations, Users will only see Machines based on their Role Privileges
* In Schedule Operations, Machine Privileges are not applied

![](../static/img/Machine_Privileges-1c4bd6483644900832ba6ecbbeb06a95.png)

### Schedule Privileges

* Removes/Grants Privileges to specific Schedules
* In order to view a Schedule, each OpCon user must be granted access
    * If a User does not have access to see a Schedule, that User would never know it exists
* If a User creates a Schedule, that User is automatically granted access

![](../static/img/Schedule_Privilges-398fc204c2886f989a2534f57bf6c8c5.png)

### Function Privileges

* Individual Privileges inside ‘Function Privileges’ are used to grant access to Functions not related to Jobs
* Each User must have Function Privileges via one or more Roles to perform actions within OpCon

![](../static/img/Activities-83ab769adac3172955edc4c20d8f5b65.png)

### For More Information

**[Privileges](https://help.smatechnologies.com/opcon/core/administration/privileges)**

**[Access Management](https://help.smatechnologies.com/opcon/core/Files/UI/Solution-Manager/Library/AccessManagement/Access-Management)**

**[Managing Privileges](https://help.smatechnologies.com/opcon/core/Files/UI/Solution-Manager/Library/AccessManagement/Roles/Managing-Roles-And-Privileges)**