---
sidebar_label: 'Practice: Create Dependencies'
---

# Practice: Create Dependencies

### Objective

Create a **REQUIRES** Dependency Chain for the four Jobs in **Schedule 1**. 

The Dependency Flow should be:

**Windows Job 1** <- **Windows Job 2** <- **Windows Job 3** <- **Windows Job 4**

where **Windows Job 4** Requires **Windows Job 3**, etc.

### Instructions

1.	In Solution Manger, select **Studio**. 
2.	In the **Schedule** list, select **Practice Schedule 1e**.
3. Click the **View** button.
3.	Click **Windows Job 4**.
4.	In the Job menu, click **Add Dependency**.
5.	In the **Schedule** Schedule frame, check that **Schedule 1** is selected.
6.  In the **Job** drop down list, select **Windows Job 3**.
7.	In the **Dependency** frame, select **Requires** and **Finished OK**.
8.	Click **Windows Job 3**.
9.	In the Job menu, click **Add Dependency**.
10.	In the **Schedule** Schedule frame, check that **Schedule 1** is selected.
11.  In the **Job** drop down list, select **Windows Job 2**.
12.	In the **Dependency** frame, select **Requires** and **Finished OK**.
13.	Click **Windows Job 2**.
14.	In the Job menu, click **Add Dependency**.
15.	In the **Schedule** Schedule frame, check that **Schedule 1** is selected.
16.  In the **Job** drop down list, select **Windows Job 1**.
17.	In the **Dependency** frame, select **Requires** and **Finished OK**.
