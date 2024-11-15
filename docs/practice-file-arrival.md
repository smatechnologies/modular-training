---
sidebar_label: 'Practice: File Arrival'
hide_title: 'true'
---

# Practice: File Arrival

### Objective

Use File Arrival to detect the arrival of a file.

### Instructions

#### Create a Blank File

1. In the Windows directory, create a new folder named ```C:\Windows File Arrival```.
2. Within the new folder, create a blank text file named ```WindowsFile1.txt```.

#### Create the Schedule

3. Open** Solution Manager**.
4. In **Library** > **Administration**, select on **Master Schedule**. 
5. Click the **Add** button.
6. On the **Master Schedule Definition** screen:
* In the **Name** field, provide a Name for the Schedule.
* Add **Documentation**
* Select working days.
* Configure **Auto Build** and **Auto Delete**.
* Click **Save**
7. Click **Back**

#### Create the File Arrival Job

8. Select the **Windows File Arrival** schedule in **Schedule List** and click the **View** button.
9. Select **Add Job** in the side menu 
10. On the **Master Schedule Definition** screen:
* In the **Name** field, enter the desired Job Name.
* In the **Job Type** drop-down, select **Windows**
* In the **Machine Selection**drop-down, select the desired Machine.
* In the **User ID** drop-down, select the desired USER ID.
* In the **Job Action** drop-down, select **File Arrival**
* In the **File Name** field, enter ```"C:\Windows File Arrival\WindowsFile1.txt"```
* In the **Start Time** drop-down, enter 0 day at ```08:00 AM```
* In the **End Time** drop-down, enter 0 day at ```06:00 PM```
* In the **File Size Stable Duration (in secs)** drop-down, enter ```5```
11. Add **Documentation** to the Job.
12. Give the Job a **Frequency** of **Mon-Fri-N**
13. click **Back**

#### Build the Schedule

14. Build the Schedule **Released** for today.
15. In **Processes**, view the Schedule and verify that the **Windows File Arrival Job** is running. 
16. Once the Job runs, verify that the Job was created and that the file was found by inspecting the **Job Output**.

### Video Walkthrough

[![File Arrival](../static/img/file-arrival.png)](https://sma1980-my.sharepoint.com/:v:/g/personal/rweesner_smatechnologies_com/Eatr4YcXitNArCGfw5qq-aYBtpjnudcmGkphAxCrgFDIVQ?e=r28nBE&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D)



