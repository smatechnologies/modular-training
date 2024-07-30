---
sidebar_label: 'Practice: Create A Resource'
hide_title: 'true'
---

# Practice: Create A Resource

### Objective

To use a Resource in order to prevent multiple jobs from kicking off at the same time.

### Instructions

#### Create the Resource

1.	In **Library** > **Administration**, select **Resources**. 
2.	Click the **Add** button.
3.	In the **Resources** pop-up:
  * In the **Name** field, enter ```TrainingResource```.
  * In the **Description** field, enter in some documentation.
  * In the **Maximum** field, enter a value of ```4```.
  * Click the **Save** button.
4.  Click **Back**.

#### Create the Schedule

5.	In **Library** > **Administration**, select **Master Schedules**.
6.	Click the **Add** button.
7.	On the **Master Schedule Definition** screen:
  * In the **Schedule Name** field, enter ```Resource Schedule```.
  * Add **Documentation** to your Schedule.
  * Monday through Sunday are working days
  * Do **NOT** use the Master Holiday Calendar.
  * **Auto Build** ```7``` days in advance for ```1``` days
  * **Auto Delete** ```7``` days ago
  * Click the **Save** button.
8.  Click **Back**.
9.	Select **Resource Schedule** in the **Schedule List**,
10. Click **View**.

#### Create the Jobs

11.	Select **Add Job** button in the side menu.
12.	On the **Master Job Definition** screen, 
  * In the **Name** field, enter ```Use 2 Job A```.
  * In the **Job Type** drop down, select **Windows**.
  * In the **Machine Selection** section, select the desired machine from the **Machines or Machine Group** drop down. 
  * In the **General** section, select the desired user from the **User Id** drop down.
  * Under the **Run** section, **type** the following in the **Command Line** box:
```cmd
timeout /t 10
```
  * Click the **Save** button.
13. Click the **Lock** icon to enter **Admin Mode**.
14. In the **Documentation** section, add some **documentation**.
15. In the **Frequency** section, create or add desired Frequency. Click **Save**.
16. Click **Back**.
17. Utilizing the **Copy** function, copy job **Use 2 Job A** to create **Use 2 Job B** and **Use 4 Job**.

#### Create the Resource Dependency

18.	In **Studio**, select **Use 2 Job A**
19. In the side panel, select **Add Resource Dependency**
20. In the **Resource** pop-up:
  * In the **Resource** drop down, select **TrainingResource**.
  * In the **Value** textbox, enter ```2```.
  * Click the **Save** button
  * Click the **Save** button in **Master Job Definition**
21. Repeat **Steps 18-20** to add the **Resource Dependency** of **2** to **Use 2 Job B**.
22. Repeat **Steps 18-20** to add the **Resource Dependency** of **4** to **Use 4 Job**.
23. Close **Library**
24. Close **Studio**.

#### Create the Notification

25. In **Library** > **Management**, select **Notification Triggers**.
26. Select **Manager Groups**.
27. On the **Manage Groups** screen, click **Add**.
  * In the **Name** field, enter ```TrainingResource```
  * In the **Type** dropdown, select **Schedule**.
  * In the **Schedule List**, select **Resource Schedule**.
  * Click **Save**.
28. Return to the **Notification Triggers** main screen.
29. Click **Add**.
30. In the bottom of the **Notification Triggers** screen:
  * In the **Group Name** dropdown list, select **TrainingResource**.
  * In the **Trigger Name** dropdown list, select **Job Running**.
  * Click the **+** button for an **Email** alert.
  * In the **Email** pop-up window:
    * In the **To** field, enter *desired email* (or property if you created one).
	* In the **Subject** field, enter ```Resources in Use for TrainingResource when [[$JOB NAME]] is running```
	* In the **Message** field, enter ```Number of Resources for resource TrainingResource => [[RU.TrainingResource]]/[[RM.TrainingResource]]```
	* Click the **OK** button.
  * Click the **Save** button.
31. Close **Library**.

#### Build the Schedule

32.	Build the Schedule Released for today and view the Schedule and Job results in **Processes**.
33.	Be sure the **Resource Schedule** is Completed
34. Open the email client and check the inbox. You should find `3` new emails.
35. Close **Operations**

### Video Walkthrough

[![Create A Resource](../static/img/create-a-resource.png)](../static/video/create-a-resource.mp4)
