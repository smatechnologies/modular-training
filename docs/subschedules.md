---
sidebar_label: 'SubSchedules'
hide_title: 'true'
---

# SubSchedules and Container Jobs

### SubSchedule: Definition

* Schedule which can be embedded in another Schedule (or other Schedules)
	* Only built if called by a Container Job
	* Give Job-like properties to Schedules
* Are Multi-Instance by default
	* Can duplicate blocks of Jobs from a shared Resource

### SubSchedule Visualization

![](../static/img/424-954afd659bb2a8bbe8ae42d63978b177.png)

### Container Job: Definition

* Job that contains Sub-Schedule
* Grants SubSchedule all Job-like properties
	* Frequencies 
    :::tip
    **Remember**: Container Jobs are **JOBS**. Jobs need Frequencies to run!
    :::
	* Time Offsets (Other Frequency Details)
	* Dependencies
	* Events
	* Etc.
* Multiple Container Jobs can reference same SubSchedule
* Container Job will only Complete if all Jobs in SubSchedule have completed

### SubSchedule/Container Job: Setup

* Create SubSchedule:
	* Create Schedule in Schedule Master
	* Mark Schedule as **SubSchedule**
* Embed SubSchedule within another Schedule by creating Container Job
	* Create Job using Container Job Type
	* Select SubSchedule that the Container Job will use

### SubSchedule Usage Scenarios

### Scenario 1 - Multiple Runs/SubSchedule

* Same 5 Job processes needs to run exact same way 4 times each day
	* Instead of Looping Jobs or Events, use **SubSchedules**

![](../static/img/429-c6cc99cb601039507fec3f6f681d329b.png)

### Scenario 2 - Concurrent Processes

* 5 files need to be processed by arrival time
* No order for when each file needs to be processed
* Same set of jobs will process the files
* Files need to be processed one at a time

![](../static/img/430-15225595dc701689e147b4b969caddc1.png)

### Scenario 3 - Daily and Monthly Process

* Daily Schedule has 5 processes that must run every working day
* If it is end of month, instead of running these 5 processes, Monthly Schedule, with 7 processes, must run **excluding** execution of Daily Schedule

![](../static/img/431-60ee46deec671878b60e14b35d0173f0.png)

### Scenario 3 - Daily and Monthly Process Solution

* Create Schedule with 2 SubSchedules
	* Daily SubSchedule with 5 jobs
	* Monthly SubSchedule with 7 jobs
	* Main Schedule will have both SubSchedules as Container jobs
	* Monthly Schedule has **Excludes Dependency** on Daily SubSchedule
    
:::note
This solution simplifies Frequencies definitions
:::

### Container Job Schedule Path in Job Definition

![](../static/img/sm-subschedule-schedule-path-job-definition-9b5ed9ae5cb8f702a4e66a4f8b8935cc.png)

### Container Job Task Details

![](../static/img/sm-subschedule-in-job-definition-03c59afecc8dbac4dbe66d8719ce76d3.png)

### Container Job Details in Job Summary

![](../static/img/sm-subschedule-details-job-summary-f610413325f9a937aaa52e9277e50a72.png)

### Practice Activity

**<a href="practice-subschedules" target="_blank">SubSchedules</a>**

### For More Information

**[SubSchedules and Container Jobs](https://help.smatechnologies.com/opcon/core/operations/containers)**

**[Container Job Type](https://help.smatechnologies.com/opcon/core/job-types/container)**

**[Viewing SubSchedules in Canvas](https://help.smatechnologies.com/opcon/core/Files/UI/Solution-Manager/Studio/Canvas/Viewing-Master-Schedules/#subschedules)**

**[SubSchedule Names](https://help.smatechnologies.com/opcon/core/operations/schedule-names#subschedules)**
