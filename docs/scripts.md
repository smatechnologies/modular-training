---
sidebar_label: 'Embedded Scripts'
hide_title: 'true'
---

# Embedded Scripts

* OpCon has ability to push Scripts from the OpCon database to Windows and UNIX environments
* The OpCon Database acts as a centralized Repository that is replicated with database
* The Repository allows for Version Control

![](../static/img/sm-scripts-ed7b63a6d67f1d6cf97e01d7a07e60c3.png)

#### Four part make up Embedded Scripts

* Script Types
* Script Runners
* Script Repository
* Job Master

### Script Types

* Configure type of Scripts which can be stored by OpCon
* *There are 6 **predefined** Script types, but more can be added*
  * Command Shell (.cmd)
  * Perl (.ps)
  * PowerShell (.ps1)
  * Python (.py)
  * VBScript (.vbs)
  8 SQL (.sql)

![](../static/img/sm-script-types-8356caec36fcc18417ce92cb7f2559aa.png)

### Script Runners

* Script Runners define Command Line created to run Script
* Allows more than one Script runner per Script Type

:::tip Example
* Powershell would include ```“–ExecutionPolicy Bypass and –File”``` before command, so the Script Runner would look like: ```powershell.exe -ExecutionPolicy Bypass -File $FILE $ARGUMENTS```.
:::

![](../static/img/sm-script-runners-c40c693849b0f9599e8ece1e00e30533.png)

### Script Repository

* Where Scripts are created and stored
* Previous versions are accessible

![](../static/img/sm-add-script-cc4aa3d08d298a76b61aba64c66413b4.png)

#### Required Fields

* **Name** – Defines Name of Script (No spaces allowed in Name)
* **Description** – Documents purpose of Script
* **Open File** - Allows loading of Script from network
* **Blank Text Field** – Create Script 
* **Type** – Specifies Script Type 
* **Initial Comments** – Documents differences between Script versions

#### Assign a Role to a New Script

* A Role must be assigned when a Script is created or imported to the Script Repository

![](../static/img/sm-assign-role-script-d23885ad95897ee3d2fbde39f952d602.png)

#### Edit a Script

* In the Repository, a **Copy** of the script must be made before you can **Edit** it.

![](../static/img/sm-copy-script-edit-b495e6c35071f628e834cfec780ecbcf.png)

![](../static/img/sm-edit-script-version-cd1210dc51cd14c2bf914bf652f9ed60.png)

#### Deploy Script

* Multiple jobs can run differnt versions of the same Embedded script.
* To have all jobs run the same version, one needs to **Deploy** that version to the jobs.

![](../static/img/sm-deploy-script-button-988ef1145834c184254df158998a97d6.png)

![](../static/img/sm-script-deploy-2f4a88ba2691c82f95c1f9bd5ba4d603.png)

#### Script Cross References

* Cross Reference in the Repository allows one to see all the jobs that are running the same script.

![](../static/img/sm-script-cross-references-79103be519cd70265223a6c81d101075.png)

:::warning
A Script with Cross References cannot be deleted
:::

### Embedded Script Job

![](../static/img/sm-script-in-job-properties-c533528a7323c9f3812c2151557901e7.png)

* **Job Action** – Change from Run Program to Embedded Scripts
* **Script** – Specifies which script to call
* **Script Type** – Specifies Script Type for Selected Script
* **Runner** – Script Runner for Selected Script
* **Run Command Template** – Contents of Script Runner
* **Version** – Specifies Script Version selected
* **Arguments** – Enter the parameter(s) passed to Script (if needed)
* **Working Dir.** – Working Directory (starting directory) for Script

### Scripts Documentation

[Embedded Scripts](https://help.smatechnologies.com/opcon/core/automation-concepts/embedded-scripts)

[Managing Scripts](https://help.smatechnologies.com/opcon/core/Files/UI/Solution-Manager/Library/Scripts/Managing-Scripts)

[Managing Script Versions](https://help.smatechnologies.com/opcon/core/Files/UI/Solution-Manager/Library/Scripts/Managing-Script-Versions)

[Managing Script Types](https://help.smatechnologies.com/opcon/core/Files/UI/Solution-Manager/Library/Scripts/Managing-Script-Types)

[Managing Script Runners](https://help.smatechnologies.com/opcon/core/Files/UI/Solution-Manager/Library/Scripts/Managing-Script-Runners)

### Practice

<a href="practice-scripts" target="_blank">Practice - Embedded Scripts</a>