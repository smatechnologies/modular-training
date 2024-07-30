---
sidebar_label: 'Practice: Escalation Manager'
hide_title: 'true'
---

# Practice: Esclation Manager

### Objective

To set up escalation so that notifications are escalated through channels.

### Instructions

#### Create a Schedule Intended to Fail

1.  In **Library** > **Administration**, select **Master Schedule**.
2.  Click **Add** button.
3.  On the **Master Schedule Definition** screen:
  * In the **Schedule Name** field, enter ```Escalation Schedule```.
  * Auto Build ```7``` days in advance for ```1``` days.
  * Auto Delete ```7``` days ago.
  * **Save** the Schedule.
4.  In **Studio**, select **Escalation Schedule** and click **View**.
5.  In the side menu, select **Add Job**.
6. In the **Master Job Definition** screen:
  * In the **Name** field, enter ```Escalation Fail Job```.
  * In the **Job Type** drop down, select **Windows**.
  * In the **Machine Selection** section, select the desired machine from the **Machines or Machine Group** drop down. 
  * In the **General** section, select the desired user from the **User Id** drop down.
  * Under the **Run** section, **type** the following in the **Command Line** box:
 
```
"Bad Command Line to Fail"
```

  * Add **Documentation**.
  * In the **Frequency** section, create or add desired Frequency.


7.	In **Library** > **Management**, select **Escalation Manager**. 

#### Create the Escalation Group

8.	In the **Groups** section on the right side, click **Add**.
9.	In the **Add New Escalation Group** pop-up window:
  * In the **Name** field, enter ```Level 1```.
  * In the **Users** section, select desired users.
  * Click the **>** button to move the users to the **Assigned Users** column. 
  * Click the **Save** Button.

#### Create the Escalation Rule

10.	In the **Rules** section on the left side, click **Add**.
11.	In the **Add New Escalation Rule** pop-up window: 
  * In the **Name** field, type ```Escalation Job Failure```.
  * In the **Rule Sequences** section, click **Add**.
  * In the **Add New Rule Sequence** pop-up window:
    * In the **Number of Times To Be Notified** field, enter ```6```.
    * In the **Time between Notifications (minutes)**: textbox, enter ```00:05```.
    * In the **Group** drop-down, select ```Level 1```.
    * Click **Add**.
  * Click **Save**

:::info Note
If you needed to add multiple escalation levels, you would click add again on the **Add New Escalation Rule** pop-up window and follow that the same process.
:::

#### Create a Notifcation Group and Trigger

12.	In **Library** > **Management**, select **Notification Triggers**. 
13.  Click **Manage Groups** in the upper right corner.

#### Create a Notification Group

14.  On the **Manage Groups** screen, click **Add**.
15.  In the **Name** field, type ```Job Failure```.
16.  In the **Type** drop-down, select **Job**.
17.  Under the **Name** field, select **Included** so that future machines are included in this trigger.
18.  Validate that the **Selected** check boxes for both **Escalation Fail Job** is checked.
19.  Click **Save**.

#### Create the Notification Trigger

20. Click on **Notification Triggers** in the upper right corner.
21. On the **Notification Trigger** screen, click **Add**.
22. In the **Group Name** drop-down, select **Job Failure**.
23. In the **Trigger Name** drop-down, select **Job Failed**.
24. Click the **+** sign on **Email** to add an email notification.
25. In the **Email** pop-up window:
  * In the **To** field, type **desired email address**.
  * In the **Subject** field, type ```Job Has Failed```.
  * In the **Message** box, enter ```The Job Has Failed.```
  * Click the **OK** button.
26. Click **Save**.

27.	In **Library** > **Management**, select **Notification Triggers**. 
28.  Click **Manage Groups** in the upper right corner.

#### Applying the Escalation

29. Under the **Library** > **Management**, select **Notification Triggers**. 
30.	In the **Notification Triggers** section, click on **Escalation Schedule**.
31.	In the **Trigger Name** drop-down in the bottom half of the screen, validate that **Job Failed** is selected.
32.	In the **Escalation Rule** drop-down, select **Escalation Job Failure**.
33.	Click the **Save** Button.
34.	Close **Library**.

#### Build the Schedule 

35. In **Operations**, click on **Schedule Build**. 
36. Select the **Released** for today.
37. In the **Schedule List**, select **Escalation Schedule**.
38. Click the **Build** button.
39. Expand and click on the schedule link for **Escalation Schedule** to return to the **Processes** screen.

:::info Note

* The only job in the **Escalation Schedule** will fail which will triggering the **Escalation Event**.
* You will receive a pop-up alert that reads **You have notifications to acknowledge**.
* If you open your email client you should also see the initial alert, as well as another email informing you that this process has been placed in escalation.

:::

#### Acknowledge the Escalation

40. In the pop-up window that says **You have notifications to acknowledge**, click **Review**.
41. In the **Notification Acknowledgement** pop-up, check the appropriate box for the **Job Failure**.
42. Click **Acknowledge**.
43. Click **Close**
44. Close **Operations**.

:::tip
There are alternatives when acknowledging an escalation. You can also: 
* Click on the **Escalation Icon** in the lower right corner to the left of the **heartbeat**.
* Log out and back in of Solution Manager. You will get the acknowledgment alert.
:::

### Video Walkthrough

[![Escalation Manager](../static/img/escalation-manager.png)](../static/video/escalation-manager.mp4)