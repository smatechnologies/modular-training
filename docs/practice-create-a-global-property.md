---
sidebar_label: 'Practice: Create A Global Property'
hide_title: 'true'
---

# Practice: Define a Global Property

### Objective

To replace hardcoded text in the command line with a Global Property so that command line is future proofed should the value need to be changed.

### Instructions

#### Create the Global Property

1.	In the **Library** > **Administration**, select **Global Properties**. 
2.	Click the **Add** button. 
3.	In the **Name** field, enter ```RUNTIME```.
4.	In the **Value** field, enter ```10```.
5.	Add **Documentation** to the **Global Property** 
  * Example: This Global Property will store the number of seconds to run the program.
6.	Click the **Save** button on the Global Properties toolbar.
7.	Close **Library**.

#### Modify the Job

13.	Under **Library** > **Administration**, select **Master Jobs**.
14.	Using the filters, locate and select **Windows Job 1** in **Practice Schedule 1**.
15. Click the **Edit** button.
16. Click the **Lock** icon in the upper right-hand corner.
17.	Expand **Task Details**, if not already expanded.
18. Locate the **Command Line** and highlight ```10```.
19. Using either, the **Magic Wand** or **CTRL+SPACE**, pull up the **Property Selector** window.
20. Using the Search filter, locate and select the property called ```RUNTIME```.
21. Click **OK**.

:::info Note
Your updated **Command Line** should now look like:

```timeout -t[[RUNTIME]]```
:::

22.	Click the **Save** button.

23. Close **Library**.

#### Build the Schedule and Validate that the Global Property is resolved

24.	Open **Operations** and click on **Schedule Build**.
25. Validate that today is the date for the **From** and **To** fields.
26. In the **Schedule Build** section, select the **Released** radial button.
27. Select **Practice Schedule 1** from the **Schedule List**.
28. Click **Build**
29.	On the **Build Results** screen, expand the dropdown menus until you can see and click on **Practice Schedule 1**.
30.	Click the **Practice Schedule 1** link to open the Schedule in **Processes**.
31.	Verify that all Jobs **Finished OK**.
32. Right-click on one of the four jobs that were modified.
33. In the **Job Selection** panel, select **Job Output**.
34. Click **Refresh**.
35. Click on the link that appears after the **Refresh** is complete.
36. Look at lines four and five and validate that the **Global Property** resolved to ```10```
37. Close the **Job Output**.
38. Close **Operations**.


### Video Walkthrough

[![Create a Global Property](../static/img/create-a-global-property.png)](https://sma1980-my.sharepoint.com/:v:/g/personal/rweesner_smatechnologies_com/EZEaTEDG7_VGmuW6f2YT-JYBDWPeBozaCmQ035l3LmRPjA?e=vsfvFk&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D)