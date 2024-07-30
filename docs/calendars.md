---
sidebar_label: 'Calendars'
hide_title: 'true'
---

# Calendars

* In Solution Manager, **Calendars** is found in **Library > Administration > Calendars**

### Holiday Calendars

* OpCon supports several types of Calendars to help provide flexible scheduling around holidays and any other non-working days 

* **Master Holiday Calendar**
  * Installed with OpCon database
  * Stores non-working days for multiple Schedules
  * By default, there are no non-working days on this Calendar, so administrators must set any desired non-working days
  * These non-working days affect all Schedules that are configured to use the Master Holiday Calendar
* **Additional Holiday Calendar**
  * User-defined Calendars
  * Stores non-working days that can be associated with multiple Schedules
  * Administrators can create as many Additional Holiday Calendars as needed for automation
  * Non-working days on these Calendars only affect Schedules that have a Calendar selected for Additional Holidays
* **Individual Holiday Calendar**
  * Automatically created when a Schedule is initially created
  * Stores non-working days for a single Schedule
  * Administrators must set additional days as non-working days when required

* **Workdays Per Week**
    * Workdays Per Week combined with Schedule Holiday Calendars specify which dates are considered working days
    * Workdays Per Week can be overwritten by Frequencies


#### Calendar Select/Add/Edit Main Screen



#### Calendar Add/Edit Selections



#### Calendar Associations


### Calendar Documentation

[Calendars](https://help.smatechnologies.com/opcon/core/objects/calendars)

[Managing Calendars](https://help.smatechnologies.com/opcon/core/Files/UI/Solution-Manager/Library/Managing-Calendars)

### Practice

<a href="practice-calendars" target="_blank">Practice - Calendars</a>