---
slug: '/'
sidebar_label: 'Training Walkthroughs'
---

# Self-Guided OpCon Basic Training

## Overview

**OpCon** (Operations Console Cross-Platform Scheduler) is an enterprise-wide, heterogeneous workflow automation and orchestration platform.

* OpCon can be utilized to create, schedule, and execute tasks for your processes. 
    * The most basic objects implemented to execute processes are the **Schedule** and **Job**.
    * The creation of a **Schedule** helps to identify a group of one or more **Jobs** (tasks) that can be executed.  
* OpCon allows for **Jobs** to be grouped together in workflows with **Dependencies** and **Events** to trigger desired behaviors.
    * **Jobs** can be created with any **Frequency** (specified dates, times, and intervals to run).   
* In OpCon, a "master" **Schedule** and "master" **Job** create the framework for future iterations of the same Schedule and Job to run daily based on a configured **Frequency** and/or **Calendar**.  
* When a **Schedule** and **Job** have been created, the final step is the **Build** process, which creates a data field indicating that the **Schedule** and **Job** will run based on the **Frequency** assigned.

---

The content contained in this repository provides a self-guided basic training program for SMA OpCon. The training covers important concepts with the following tools:

* Basic informational content
* Links to official documentation
* Practice activities 
* Walkthrough videos

:::info Note 

The **Practice** activities within this training assume users have an OpCon environment in which they can be completed.

:::

*Below you will find Walkthrough Videos for each topic including a link to the informational and practice section for that topic.*

### Schedule and Job Basics

<div class="grid-container">

<div class="grid-item">

[![Create a Machine](../static/img/create-a-machine.png)](https://sma1980-my.sharepoint.com/:v:/g/personal/rweesner_smatechnologies_com/EQ42_awqYo9Inv3YznEcRB0BuPlNO_mniDo-eXd4ppXfzg?e=9fUSea&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D)

[Information](/training/modular-training/agents-machines)

</div>

<div class="grid-item">

[![Create a Schedule](../static/img/create-a-schedule.png)](https://sma1980-my.sharepoint.com/:v:/g/personal/rweesner_smatechnologies_com/EbFcFlL7IslIvR8tKo8B5wQBMr4dph_qrPTM6xRFh8wLsg?e=1g5s8K&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D)

[Information](/training/modular-training/schedules)

</div>

<div class="grid-item">

[![Create a Job](../static/img/create-a-job.png)](https://sma1980-my.sharepoint.com/:v:/g/personal/rweesner_smatechnologies_com/EeAwW_dv9CVMldkzxBaZfeIBL1vrCEmYChpQQMAFCdq43w?e=IbHNDJ&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D)

[Information](/training/modular-training/jobs)

</div>

<div class="grid-item">

[![Create a Null Job](../static/img/create-a-null-job.png)](https://sma1980-my.sharepoint.com/:v:/g/personal/rweesner_smatechnologies_com/Eeb6So__CaRGigyMyrqeBD4ByvcKnZWmDn1CnvLmPCgBiA?e=CfaSd9&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D)

[Information](/training/modular-training/null-jobs)

</div>

<div class="grid-item">

[![Create a Frequency](../static/img/create-a-frequency.png)](https://sma1980-my.sharepoint.com/:v:/g/personal/rweesner_smatechnologies_com/EX3UVyp5CQtOqhurx5EYqr8Bl0ZFmwY9X7tKNLnDjZPTLg?e=NCCbhh&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D)

[Information](/training/modular-training/frequency-definition)

</div>

<div class="grid-item">

[![Build a Schedule](../static/img/build-a-schedule.png)](https://sma1980-my.sharepoint.com/:v:/g/personal/rweesner_smatechnologies_com/Eaqm_dC-oM9KjKTU-67pS68BnHLGiv3ReQMDKTnYp5_JsQ?e=Gi5hij&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D)

[Information](/training/modular-training/schedule-build)

</div>

<div class="grid-item">

[![Create a Job Dependency](../static/img/create-a-job-dependency.png)](https://sma1980-my.sharepoint.com/:v:/g/personal/rweesner_smatechnologies_com/EbAuaNdjMrZCvFOOYZR_MO0BqzUP4I5V71sgLrUFyrcZBg?e=e594oO&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D)

[Information](/training/modular-training/dependencies)

</div>

<div class="grid-item">

[![Create a Tag](../static/img/create-a-tag.png)](https://sma1980-my.sharepoint.com/:v:/g/personal/rweesner_smatechnologies_com/EWICgCY3oQdDlJe_u0P_meABb6L7qBhkFo1rds5Q8iLW9A?e=1Sjveq&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D)

[Information](/training/modular-training/tags)

</div>

</div>

## Operations

<div class="grid-container">

<div class="grid-item">

[![Escalation Manager](../static/img/escalation-manager.png)](https://sma1980-my.sharepoint.com/:v:/g/personal/rweesner_smatechnologies_com/EbsQDquBK31Dr3xu1Hg9ZN8B-xfHnwLgVuOBcG40n3GWPA?e=JhQISO&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D)

[Information](/training/modular-training/escalation-manager)

</div>

<div class="grid-item">

[![Notification Manager](../static/img/notification-manager.png)](https://sma1980-my.sharepoint.com/:v:/g/personal/rweesner_smatechnologies_com/ESAVRf7AJJJFoDdYt0KMKDcByC8BH-4SfIHubZP19nG28w?e=oWSjk9&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D)

[Information](/training/modular-training/notification-manager)

</div>

</div>

## Objects and Components

<div class="grid-container">

<div class="grid-item">

[![Calendars](../static/img/calendars.png)](https://sma1980-my.sharepoint.com/:v:/g/personal/rweesner_smatechnologies_com/ESAVRf7AJJJFoDdYt0KMKDcByC8BH-4SfIHubZP19nG28w?e=oWSjk9&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D)

[Information](/training/modular-training/calendars)

</div>

<div class="grid-item">

[![Create a Global Property](../static/img/create-a-global-property.png)](https://sma1980-my.sharepoint.com/:v:/g/personal/rweesner_smatechnologies_com/EZEaTEDG7_VGmuW6f2YT-JYBDWPeBozaCmQ035l3LmRPjA?e=vsfvFk&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D)

[Information](/training/modular-training/global-properties)

</div>

<div class="grid-item">

[![Embedded Scripts](../static/img/scripts.png)](https://sma1980-my.sharepoint.com/:v:/g/personal/rweesner_smatechnologies_com/EfcDkQVQFNdAu-RqbXVTJT8BjE1W1YGpSd8_1_z2xRzqcA?e=HiVoqK&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D)

[Information](/training/modular-training/scripts)

</div>

<div class="grid-item">

[![Create an Event](../static/img/create-an-event.png)](https://sma1980-my.sharepoint.com/:v:/g/personal/rweesner_smatechnologies_com/EcdBcMJOuilCuJnyAdmwPkgBd3hLtfQR2C10emhe4bdTpw?e=Dw6gol&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D)

[Information](/training/modular-training/events)

</div>

<div class="grid-item">

[![Create A Resource](../static/img/create-a-resource.png)](https://sma1980-my.sharepoint.com/:v:/g/personal/rweesner_smatechnologies_com/Ea82mw9zZTpCvcs92oDf5vABOsjNNjVhplHXty-I3Mj9nQ?e=app46H&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D)

[Information](/training/modular-training/resources)

</div>

<div class="grid-item">

[![Create A Threshold](../static/img/create-a-threshold.png)](https://sma1980-my.sharepoint.com/:v:/g/personal/rweesner_smatechnologies_com/EaLBxeK8-ldPoUjaLkyF6lEBMoSvClDnXo8cUW2ytP6IUQ?e=M6meEa&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D)

[Information](/training/modular-training/thresholds)

</div>

</div>

## Advanced Features

<div class="grid-container">

<div class="grid-item">

[![SubSchedules](../static/img/subschedules.png)](https://sma1980-my.sharepoint.com/:v:/g/personal/rweesner_smatechnologies_com/EVEU7dfRWWBLi7h33YGK8koBAs81tt7Xj7GAlbDrEbxFuw?e=Jp97dt&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D)

[Information](/training/modular-training/subschedules)

</div>

<div class="grid-item">

[![File Arrival](../static/img/file-arrival.png)](https://sma1980-my.sharepoint.com/:v:/g/personal/rweesner_smatechnologies_com/Eatr4YcXitNArCGfw5qq-aYBtpjnudcmGkphAxCrgFDIVQ?e=r28nBE&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D)

[Information](/training/modular-training/file-arrival)

</div>

</div>