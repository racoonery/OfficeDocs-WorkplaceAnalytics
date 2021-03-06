﻿---
# Metadata Sample
# required metadata

title: Workplace Analytics Setup -- Prepare and upload organizational data
description: Setup steps to prepare and upload organizational data in Workplace Analytics. 
author: madehmer
ms.author: v-leash
ms.date: 07/23/2018
ms.topic: get-started-article
localization_priority: normal 
ms.prod: wpa
---

* **Owner** - Workplace Analytics administrator, HR information system administrator, LOB system administrators, or data analyst
* **Task** - Obtain organizational data needed for analysis from other information systems
* **Outcome** - CSV file of organizational data is generated and uploaded to Workplace Analytics for final provisioning

Organizational data is the information about employees that your company provides to use in Workplace Analytics. By combining organizational data about employees with their Office 365 collaboration data, analysts can filter, group, and compare employees based on their organizational context to identify relationships between employee attributes and collaboration patterns.


### What is organizational data?

- Individual data with descriptive information about company employees
- Sourced from multiple sources
    - Human Resources Information Systems (HRIS), such as Workday or PeopleSoft
    - Payroll systems
    - Employee surveys (such as engagement, manager feedback, and culture)
    - Performance Management Systems or Quota Attainment Systems
    - CRM systems
- Workplace Analytics organizational data is structured as a flat (CSV) file with each row representing one person and columns representing attribute fields.

### How is data used?

 * Gives context for the mailbox data that enables Workplace Analytics to calculate metrics based on the relationship of the org data attributes.
 * Enables the user to filter and group data in meaningful ways and generate custom metrics.

### How often should it be refreshed?

To account for organization changes, it is recommended to refresh the data monthly.
When loading your data the first time, Workplace Analytics loads 13 months of data.  Ideally, you would load 13 dated rows of organizational data for each employee.

#### Who should be included in the org data file?

- HR Data:
    - You need organizational attributes for all employees in your company, even if they are not part of the measured population.
    - At a minimum, you need organizational attributes for all measured employees.
    - If you include business outcome data, such as engagement, productivity, and performance, you typically only need those attributes for the measured employees.

> [!Note]
> You can include up to 65 data attributes in your org data file.

> [!Important]
> To help ensure privacy, do not include employee names as an attribute.

### What are common pitfalls to avoid?

 * Too many or too few unique values
 * Redundant values
 * Attributes that only exist for a subset of your employees
 * Dirty data

### To prepare your organizational data for upload to Workplace Analytics

<!-- 
After you have created your source .csv file, you can upload it to the Workplace Analytics service. After your data has been successfully uploaded, Workplace Analytics will perform additional validation and processing to complete provisioning. The Workplace Analytics team will contact your Workplace Analytics administrator if any problems arise.
-->

* Follow the instructions in [Prepare organizational data](../Setup/Prepare-organizational-data.md), which also provides the list of required and optional organizational attributes.

After the CSV file is created, the Workplace Analytics administrator can upload it. For more information, see [Upload organizational data](../Setup/Upload-organizational-data.md).

### Video: Upload organizational data

<!-- out for now
Watch this video to learn how to upload organizational data to Workplace Analytics.
-->

<!-- old link, with thumbnail
[<img src="../Images/WpA/setup/Upload-org-data.png" alt="Upload organizational data">](https://aka.ms/WpAPrepUploadOrgData_Video)
-->

<iframe width="640" height="564" src="https://player.vimeo.com/video/282897809" frameborder="0" allowFullScreen mozallowfullscreen webkitAllowFullScreen></iframe>


After your upload is submitted successfully, additional validation and processing of your data occurs to complete provisioning. If any problems arise, the Workplace Analytics team will contact your Workplace Analytics administrator.

### After provisioning

After data is completely provisioned, Workplace Analytics users can access the full set of product features.
Office 365 meeting and email data is refreshed monthly. This is a good time for the Workplace Analytics administrator to also generate and upload updated organizational data.
