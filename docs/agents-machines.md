---
sidebar_label: 'Agents/Machines'
hide_title: 'true'
---

# Agents/Machines

### Definitions

* A Representation of an Agent **(LSAM)** in OpCon’s database
* LSAM stands for “**Local Schedule Activity Monitor**”
* LSAM/Agent listens for commands from OpCon’s main engine kicking off and monitoring specified tasks
* Machines define where a task will be run

#### Machine Status

* Displays Connection Status of all Machines configured in the OpCon database
  * Displayed in Grid format
  * Statuses are updatable from this screen


### Agent List Screen

![](../static/img/sm-agents-list-6df80df8b84d23f62914267b156338e3.png)

### Agent Details

![](../static/img/sm-agent-details-9fca23166e1f80c413cce0c397c9a8c0.png)

### Machine Groups

A **machine group** displays the user-defined machines with common characteristics and usage. All machines in a group must have a common operating system. Additionally, all machines in a group must have the same data structure for their jobs (i.e., all must be using either Non-XML or all must be using XML).

The following information applies to defining machine groups:

* **Name:** Defines the name for the machine group.
* **Machine OS Type:** Defines the OS Type for the machine group.
* **Description:** Provides an area for descriptions, explanations, and notes that can be updated for the defined machine group. in the Enterprise Manager online help.
* **Machine Assignment:** Defines all assigned machines for the defined machine group. Machines in the group must have matching operating systems and communication protocols.

![](../static/img/SM_machinegroups.png)

### Agent/Machine Documentation

[Machines](https://help.smatechnologies.com/opcon/core/objects/machines)

[Managing Agents](https://help.smatechnologies.com/opcon/core/Files/UI/Solution-Manager/Managing-Agents)

[Performing Agent Status Updates](https://help.smatechnologies.com/opcon/core/Files/UI/Solution-Manager/Performing-Agent-Status-Updates)

[Machine Groups](https://help.smatechnologies.com/opcon/core/Files/UI/Solution-Manager/Library/MachineGroups/)

### Practice

<a href="practice-create-a-machine" target="_blank">Practice - Create a Machine</a>