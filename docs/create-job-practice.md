---
sidebar_label: 'Practice: Create a Job'
---

# Practice: Create a Job

### Objective 

Create a Job named **Windows Job 1** within the schedule named **Schedule 1**. The Job must run on the ```WINDOWS``` machine type. The Job must use the ```SMATRAINING``` machine and the ```SMATRAINING\SMAUSER``` User Id. The command line should run the following program:

```timeout /t 10```

Assign the Job an **Existing Frequency** of ```Example-Mon-Sun-O```. Repeat the preceding steps to create 3 more Jobs identical to **Windows Job 1** following the same naming pattern.

### Instructions

1.	In Solution Manager, select **Studio**. 
2.	In the Schedule list, select **Schedule 1**.
3.	In the Menu to the right, select **Add Job**.
4.	In the Schedule drop-down list, select **Schedule 1**.
5.  In the Name textbox, enter **Windows Job 1**
6.  In the Job Type drop-down list, select **Windows**.
7.  Click on **Task Details** to open the Details box.
8.	In the Machines or Machine Group drop-down list, select the SMATraining machine. 
9.	In the User ID drop-down list, select ```SMATRAINING\SMAUSER```
10.	Under **Run**, in the **Command Line**, type: 

```timeout /t 10```

11.	Click the **Save** button.
12. Click the **Lock** button in the right hand corner of the Master Job Details screen.
13. Select the **Frequency** tab and select the **Add** button.
14.	Create a Frequency named ```Mon-Sun-0```.
- Select ```All Weeks``` from the **When to Schedule** dropdown.
-  Select ```Monday``` through ```Friday``` in the **Days of the Week** menu.
-  Select ```Before Date``` in the **A/O/B/N** menu.
- Click **Save**.
Create three jobs that are identical to Windows Job 1.
15. Navigate to **Library** > **Master Jobs**.
16. In the Master Jobs screen, select **Windows Job 1** 
17. Click the **Copy** button.
18. Enter the Job Name as **Windows Job 2**.
19. Deselect the "Navigate to Maser Job Definition Page after copy" option.
20. Click the **OK** button.
21. Repeat the copy process to create **Windows Job 3** and **Windows Job 4**.
22.	Close the **Job Master**.