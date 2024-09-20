---
sidebar_label: 'Practice: SubSchedules'
hide_title: 'true'
---

# Practice: SubSchedules

### Objective

To use a Resource to prevent multiple Container jobs from kicking off at the same time.

### Instructions

#### Create Resource

1. In **Library** > **Administration**, select **Resources**. 
2. Click the **Add** button.
3. In the **Resource** pop-up window:
* Provide a **Name** for the Resource. 
* In the **Description** field, enter some documentation.
* In the **Max Resources** field, enter ```1```.
* **Save**.
4. Click **Back**

#### Create Primary Schedule

5. In **Library** > **Administration**, select on **Master Schedules**. 
6. Click the **Add** button. 
7. Provide a **Name** for the Schedule. 
* In the **Documentation** field, enter some documentation
* **Save**.

#### Create the Sub-Schedule

8.	In **Library** > **Administration**, select on **Master Schedules**. 
9.	Click the **Add** button. 
10. On Master Schedule Definition screen:
* Provide a **Name** for the SubSchedule. 
* In the **Schedule Settings** frame, mark the **SubSchedule** checkbox.
* Click the **Save** button.

#### Create Container Jobs

11. In **Library** > **Administration**, select on **Master Schedules**.
12. Select the **Process Files** Schedule.
13. Select **View**.
14. Select **Add Job** in the side menu.
15. On the Master Job Definition screen create a Container Job:
* Provide a **Name** for the Container Job. 
* In the **Job Type** dropdown, select **Container**.
* On the **Master SubSchedule** dropdown, select the newly created **Subschedule**.
* Click the **Save** button.
* Click the **Lock** icon in the upper right-hand corner.
* Scroll to and expand the **Frequency** box.
* Select or Create a desired **Frequency**.
* In the **Add Resource Dependency** section select the previously created **Resource** 
* Enter the value of ```1``` and **Save**.
* Click **Save**.
16. Utilizing the **Copy** feature, copy the first Job until you have 5 new Jobs with a similar naming convention.


#### Build the Schedule

20.	In **Operations**, build the Primary Schedule **released** for today and check the results.


### Video Walkthrough

[![SubSchedules](../static/img/subschedules.png)](https://sma1980-my.sharepoint.com/:v:/g/personal/rweesner_smatechnologies_com/EVEU7dfRWWBLi7h33YGK8koBAs81tt7Xj7GAlbDrEbxFuw?e=3WUYzK&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D)