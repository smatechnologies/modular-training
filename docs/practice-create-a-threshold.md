---
sidebar_label: 'Practice: Create A Threshold'
hide_title: 'true'
---

# Practice: Create A Threshold

### Objective

To use a Threshold to trigger a job to run and use Notifications to let you know that the threshold is incrementing and decrementing.

### Instructions

#### Create the Threshold

1.  In **Library** > **Administration**, select **Thresholds**. 
2.  Click **Add**.
3.  In the **Thresholds** pop-up:
  * In the **Name** field, enter ```TrainingThreshold```.
  * In the **Value** field, enter a value of ```0```.
  * In the **Description** field, enter in some documentation.
  * Click the **Save** button.
4.  Click **Back**.

#### Create the Schedule

5.  In **Library** > **Administration**, select **Master Schedule**.
6.  Click **Add** button.
7.  On the **Master Schedule Definition** screen:
  * In the **Schedule Name** field, enter ```Threshold Schedule```.
  * Add **Documentation**
  * **Monday - Sunday** are working days.
  * Do **NOT** use the Master Holiday Calendar.
  * Auto Build ```7``` days in advance for ```1``` days.
  * Auto Delete ```7``` days ago.

#### Create the Jobs

8.  In **Studio**, select **Threshold Schedule** and click **View**.
9.  In the side menu, select **Add Job**.
10. In the **Master Job Definition** screen:
  * In the **Name** field, enter ```Threshold Dependency Job```.
  * In the **Job Type** drop down, select **Windows**.
  * In the **Machine Selection** section, select the desired machine from the **Machines or Machine Group** drop down. 
  * In the **General** section, select the desired user from the **User Id** drop down.
  * Under the **Run** section, **type** the following in the **Command Line** box:
 
```cmd
timeout /t 10
```

  * Add **Documentation**.
  * In the **Frequency** section, create or add desired Frequency.
11. Click **Back** to get back to the **Studio**.
12. Utilizing the **Copy** function, copy **Threshold Dependency Job** to add a second job called, **Threshold Update Job**.

#### Create Threshold Dependencies and Updates

13. In **Studio**, select the **Threshold Dependency Job**.
14. In the side menu, select **Add Threshold Dependency**.
15. In the **Threshold** pop-up window:
  * In the **Threshold** drop down, select **TrainingThreshold**.
  * In the **Operator** drop down, select **=**.
  * In the **Value** field, enter ```2```.
  * Click **Save**.
16. In **Studio**, select the **Threshold Dependency Job**.
17. In the side menu, select **Add Threshold Update**.
18. In the **Threshold** pop-up window:
  * In the **Threshold** drop down, select **TrainingThreshold**.
  * In the **Job Status** drop down, select **Finish OK**.
  * In the **Value** field, enter ```0```.
  * Click **Save**.
  * Click **Back**.
19. In **Studio**, select the **Threshold Update Job**.
20. In the side menu, select **Add Threshold Update**.
21. In the **Threshold** pop-up window:
  * In the **Threshold** drop down, select **TrainingThreshold**.
  * In the **Job Status** drop down, select **Finish OK**.
  * In the **Value** field, enter ```2```.
  * Click **Save**.

#### Create NULL Jobs and Define the Notify Events

22. In the side menu in **Studio**, select **Add Job**
23. On the **Master Job Definition** screen:
  * In the **Name** field, enter ```Initial Value Notification```.
  * In the **Job Type** field, leave it as **Null Job**.
  * Add **Documentation**.
  * In the **Frequency** section, create or add the desired Frequency.
  * Click **Save**.
24. Click **Back** to get back to the **Studio**. 
25. Utilizing the **Copy** function, copy the **Initial Value Notification** job to create 2 more jobs. One called, **After Update Job** and the other called **Final Value Job**.
26. Select the **Initial Value Notification**, click the **Wrench** icon and enter **Admin Mode**. 
  * In the **Event** section, click **+**
  * In the **Event** pop-up window:
    * In the **Send Event On** dropdown, select **Job Status**.
    * In the **Job Status** dropdown, select **Finished OK**.
    * In the **Event Template** dropdown, select ```$NOTIFY:EMAIL``` and update the **Events parameters** as follows:
	  * In the **To**, enter *desired email*.
	  * In the **Subject**, enter ```Initial value of TrainingThreshold```
	  * In the **Message**, enter ```Initial value of TrainingThreshold is [[TH.TrainingThreshold]]```
    * Click the **Save** button.
  * Click the **Save** button in **Master Job Definition**.
  * Click **Back**
27. Select the **After Update Job**, click the **Wrench** icon and enter **Admin Mode**. 
  * In the **Event** section, click **+**
  * In the **Event** pop-up window:
    * In the **Send Event On** dropdown, select **Job Status**.
    * In the **Job Status** dropdown, select **Finished OK**.
    * In the **Event Template** dropdown, select ```$NOTIFY:EMAIL``` and update the **Events parameters** as follows:
	  * In the **To**, enter *desired email*.
	  * In the **Subject**, enter ```After the Update```
	  * In the **Message**, enter ```After the update the value of TrainingThreshold is [[TH.TrainingThreshold]]```
    * Click the **Save** button.
  * Click the **Save** button in **Master Job Definition**.
  * Click **Back**
28. Select the **Final Value Job**, click the **Wrench** icon and enter **Admin Mode**. 
  * In the **Event** section, click **+**
  * In the **Event** pop-up window:
    * In the **Send Event On** dropdown, select **Job Status**.
    * In the **Job Status** dropdown, select **Finished OK**.
    * In the **Event Template** dropdown, select ```$NOTIFY:EMAIL``` and update the **Events parameters** as follows:
	  * In the **To**, enter *desired email*.
	  * In the **Subject**, enter ```Final value of TrainingThreshold```
	  * In the **Message**, enter ```Final value of TrainingThreshold is [[TH.TrainingThreshold]]```
    * Click the **Save** button.
  * Click the **Save** button in **Master Job Definition**.
  * Click **Back**

#### Add Job Dependencies

29. Select the **Final Value Job**, click **Add Dependency** in the side menu.
30. In the **Job Dependency** pop-up window, select **Threshold Dependency Job**.
31. Click **Save**.
32. Select the **After Update Job**, click **Add Dependency** in the side menu.
33. In the **Job Dependency** pop-up window, select **Threshold Update Job**.
34. Click **Save**.
35. Select the **Threshold Update Job**, click **Add Dependency** in the side menu.
36. In the **Job Dependency** pop-up window, select **Initial Value Notification**.
37. Click **Save**.

#### Build the Schedule

38. In **Operations**, build the Schedule **Released** for today.
39. Be sure the **Threshold Schedule** is **Completed**.
40. Open the email client and check the inbox.
41. You should find ```3``` new emails. Open the emails and check the contents.

:::tip

Once all the dependencies and events have been configured, your workflow should look something like this:

![](../static/img/Threshold_studio.png)

:::

### Video Walkthrough

[![Create A Threshold](../static/img/create-a-threshold.png)](https://sma1980-my.sharepoint.com/:v:/g/personal/rweesner_smatechnologies_com/EaLBxeK8-ldPoUjaLkyF6lEBMoSvClDnXo8cUW2ytP6IUQ?e=QkzzdX&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D)
