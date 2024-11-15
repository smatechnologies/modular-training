---
sidebar_label: 'Resources'
hide_title: 'true'
---

# Resources

* **Resource**: user-defined value consisting of name and numeric limit
* Resources are used to manage and limit the number of concurrently running Jobs across Schedules and Machines in OpCon
* **Max Concurrent Jobs** in Advanced Machine Properties limits the number of concurrently running Jobs on a specific Machine

	* **All** Resources can be set for Dependencies  
	* SAM is responsible for keeping track of Resources in use

:::info Note

If all Resources are in use, SAM waits until a Resource is available before submitting the next Job

:::

## Solution Manager

* In Solution Manager, **Resources** is found in **Library > Administration > Resources**

![](../static/img/sm-resources-main-8268da4880417c9d623d4d129e16c239.png)

### Create/Edit Resource

![](../static/img/sm-resource-add-d8b955250d2a5ada9e6bc5809ed216fd.png)

### Resource Dependencies in Job Details

![](../static/img/sm-resource-job-screen-ac230334b46e0212dcaba10a26117fd0.png)

### Edit/Set Resource Dependency

![](../static/img/sm-resource-dependency-add-dd22f0a3630dfde9af6c65e7ff035dc5.png)

### Trigger Email Alert of Resource Properties

![](../static/img/sm-resource-properties-1bd3b09ef07576b5e839f5371b029ecd.png)

![](../static/img/sm-resource-properties-email-5e73defd574abbfd75518d7092caeb03.png)

### Frequency - SAM Priority

* Used if Max Concurrent of the following two features is met:
	* Machine has reached Max Jobs limit (Windows and UNIX defaults are ```50```)
	* A Resource has all Resources in use
* The Job with highest **SAM Priority** will run first if several Jobs are waiting for a Resource or a Machine Max Job to free up

![](../static/img/sm-sam-priority-job-screen-aceca794e79c4c6015fc79d56079e47a.png)

### Practice Activity

**<a href="practice-create-a-resource" target="_blank">Create a Resource</a>**

### For More Information

**[OpCon Objects - Resources](https://help.smatechnologies.com/opcon/core/objects/resources)**

**[Threshold/Resource Updates](https://help.smatechnologies.com/opcon/core/job-components/threshold-resource-updates)**

**[Treshold/Resource Dependencies](https://help.smatechnologies.com/opcon/core/job-components/threshold-resource-dependencies)**

**[Solution Manager - Resources](https://help.smatechnologies.com/opcon/core/Files/UI/Solution-Manager/Library/Resources/)**



