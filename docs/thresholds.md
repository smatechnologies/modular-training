---
sidebar_label: 'Thresholds'
hide_title: 'true'
---

# Thresholds

* User-defined placeholder 
* Consists of a name and a numeric value 
* Help resolve dependencies that cannot be resolved by Job Dependency 
	* (i.e. – A specification can be made for a Job to not start until a Threshold condition is met)

### Usage

* Create a Threshold
* Assign Threshold Dependencies
* Create a trigger updating Threshold
* Reset Threshold to initial value once complete

### Threshold Dependencies

* The Threshold/Resource Dependency tab allows the definition and maintenance of Job Dependencies on Threshold and Resource values 
	* A Threshold can be used to start a Job after a certain value is reached

* In Solution Manager, **Thresholds** is found in **Library > Administration > Thresholds**

### Create/Edit Threshold

![](../static/img/sm-thresholds-add-cc34578846706778328ef8c0deeb7183.png)

#### Threshold Options in Job Details

![](../static/img/sm-thresholds-job-e39f6fd742eb813dcbf742d592272848.png)

### Threshold Update

![](../static/img/sm-thresholds-update-7218e80996700365d0d9f665997a1c10.png)

#### Threshold Dependencies

![](../static/img/sm-thresholds-dependency-5fa6c04f37f88daee0b71d8e2910835c.png)

#### Threshold Instance Properties

* Current value of Threshold can be retrieved: ```[[TH.ThresholdName]]```

#### Threshold Email Alerts

![](../static/img/sm-threshold-properties-notification-3d0eaa9e088414528a00556de6a0ed28.png)


![alt text](../static/img/sm-threshold-email-result-f592ca84531c13f87c811536ef85b9f5.png)

### Practice Activity

**<a href="practice-create-a-threshold" target="_blank">Create a Threshold</a>**

### For More Information

**[OpCon Objects - Thresholds](https://help.smatechnologies.com/opcon/core/objects/thresholds)**

**[Threshold/Resource Updates](https://help.smatechnologies.com/opcon/core/job-components/threshold-resource-updates)**

**[Treshold/Resource Dependencies](https://help.smatechnologies.com/opcon/core/job-components/threshold-resource-dependencies)**

**[Solution Manager - Thresholds](https://help.smatechnologies.com/opcon/core/Files/UI/Solution-Manager/Library/Thresholds/)**


