---
sidebar_label: 'Practice: Embedded Scripts'
hide_title: 'true'
---

# Practice: Embedded Scripts

### Objective

Use an embedded script to create a folder.

### Instructions

#### Create a Script in the Repository

1. In **Library** >> **Administration**, select **Scripts**.
2. Click the **Add** button on the toolbar.
3. In the **Name** textbox, enter **Make_Directory**.
4. In the **Type** textbox, choose **Command Shell**.
5. In the **Description** enter **Create a new folder**.
6. In the Script file section type the following (this is the example script we will run in OpCon):

```mkdir %1```

7. Click **Save**.

#### Create the Schedule

8.	From the **Home** tab, select **Studio**.   
9.	Click the **Add** button on the toolbar.   
10.	In the Schedule Name textbox, enter **Script Practice Schedule**.   
11.	In the Documentation textbox, enter **This is a Training Schedule**.  
12.	In the **Schedule Build and Maintenance** frame, mark the **Auto Build** checkbox.  
13.	Set ```7``` for the number of days in advance for Auto Build.  
14.	Set ```1``` for the number of days to Auto Build.  
15.	Mark the **Auto Delete** checkbox.  
16.	Set ```7``` for the number of days to Auto Delete.  
17.	Click the Save button.   

#### Create the Embedded Script Job

18.	In **Studio**, with **Script Practice Schedule** selected, click the **Add Job** button on the side menu. 
19.	In the **Name** textbox, enter ```Create New Folder```.
20.	In the **Job Type** drop-down list, select **Windows**.
21.	In the **Machine Selection** section, select the desired machine from the **Machines or Machine Group** drop down. . 
22.	In the **General** section, select the desired user from the **User Id** drop down.
23.	In the **Job Action** drop-down list, select **Embedded Script**.
24.	In the **Script** drop-down list, select the **Make_Directory**. 
25.	Leave the Version as **LATEST (X)**.
26.	In the **Runner** drop-down menu, select **Command Shell**.
27.	In the **Arguments** textbox, type the following, ```“C:\Backup\[[$SCHEDULE DATEYYYYMM]]”```
28.	Click **Save**.
29. Click the **Lock** icon in the upper right-hand corner.
30.	Scroll to the **Frequency** sections and create or use desired Frequency.
31.	Add **Documentation** and then click **Save**.

#### Build Schedule

32.	Build the **Script Practice Schedule** for today (Be sure to build as **Released**).
33.	Once the Job completes successfully, verify that the folder was created in **Windows File Explorer**.

### Video Walkthrough

[![Embedded Scripts](../static/img/scripts.png)](https://sma1980-my.sharepoint.com/:v:/g/personal/rweesner_smatechnologies_com/EfcDkQVQFNdAu-RqbXVTJT8BjE1W1YGpSd8_1_z2xRzqcA?e=eZQUn4&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D)