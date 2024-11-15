---
sidebar_label: 'Practice: Create A Job'
hide_title: 'true'
---

# Practice: Create a Job

### Objective 

Create a Job named **Windows Job 1** within the schedule named **Practice Schedule 1**. 

### Instructions

1.	In Solution Manager, select **Studio**. 
2.	In the **Schedule List**, select **Practice Schedule 1**.
3.	Click the **View** button in the toolbar.
4.	In the **Menu** to the right, select **Add Job**.
5.  In the **Name** textbox, enter **Windows Job 1**
6.  In the **Job Type** drop-down list, select **Windows**.
7.  Expand the **Task Details** section to open the Details box.
8.	In the **Machine Selection** section, select the desired machine from the **Machines or Machine Group** drop down. 
9.	In the **General** section, select the desired user from the **User Id** drop down.
10.	Under the **Run** section, **type** the following in the **Command Line** box:
```cmd
timeout /t 10
```
11.	Click the **Save** button.
12. Click the **Lock (or CTRL + Alt + A)** button in the top right-hand corner of the **Master Job Details** screen.
13. Scroll down and expand the **Frequency** section.
14. Click the **Add** button.
15. Name the Frequency **Mon-Sun-O**.
16. In the **When to Schedule** section, select **All Weeks**.
17. In the **Days of the Week** section, select all of the days.
18. In the **A/O/B/N** flag section, select **On Date**.
19. Leave all other options the same.
20. Click **Save**.  
21. Close **Studio** and **Library**.

### Video Walkthrough

[![Create a Job](../static/img/create-a-job.png)](https://sma1980-my.sharepoint.com/:v:/g/personal/rweesner_smatechnologies_com/EeAwW_dv9CVMldkzxBaZfeIBL1vrCEmYChpQQMAFCdq43w?e=IbHNDJ&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D)