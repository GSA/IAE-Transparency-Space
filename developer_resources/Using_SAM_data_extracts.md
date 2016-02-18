---
layout: dev_resources
title: Using SAM Data Extracts
nav: using_SAM_data_extract
---
### About SAM Data Extracts
SAM Processes **Entity Management** extract files and **Exclusion** extract files for you to download and consume into your local applications. <br>

The Entity Management extract contains information related to a Registration of an Entity including Core Data, Points of Contacts, Representations and Certifications, and other data elements depending on your level of access. <br>

The Exclusions extract contains a list of all currently open exclusions in SAM. This identifies 
entities that are in some way restricted from doing business with the US Federal Government. 

####Extract file processing times:

Monthly extract files are processed on the 1st Sunday of each month. The monthly files contain all active SAM records and SAM records that have become Expired within the last 6 months. 

Daily extract files are processed Tuesday - Saturday of each week. The daily files contain records that have been updated since the last daily file was processed. 


### Where to get SAM Data Extracts 
SAM hosts the extract files on our SFTP server and on the sam.gov site.

1. SFTP - [Click here](https://github.com/GSA/IAE-Architecture/blob/master/as-is/tech-docs/SAM/Guide%20to%20Downloading%20SAM%20Extracts%20via%20SFTP%20Site.pdf?raw=true) for How to Download SAM Extracts from the SFTP server
2. SAM.gov website. Go to [SAM.gov](https://www.sam.gov/) under the "Data Access" area and you will find all of the extract files.

**SAM Extract files are available at three access levels:**

1. **Public** (includes name, address, Point of Contact information, etc.)
2. For Official Use Only (**FOUO**) (includes certain types of Point of Contact Information and Federal Hierarchy information)
3. **Sensitive** (includes banking information and MPIN)

If you require either **FOUO** or **Sensitive** levels of access you will need to add a role to your SAM account. To do that [click here](http://gsa.github.io/openIAE/developer_resources/Access_SAM_data.html) for instructions.


**Tools available:**

| Tool Name | Description |
|---|---|
| [SAM Extract Mappings v1.0](https://github.com/GSA/IAE-Architecture/tree/master/as-is/tech-docs/SAM/SAMWebServicesExtractsMappingsv1.0) | Description of field mappings, data types, etc. |
| [Database load scripts for extracts](https://github.com/GSA/IAE-Architecture/tree/master/as-is/tech-docs/SAM/ExtractLoadScripts) | Use these scripts when you are setting up your database to consume SAM Extracts. |
| [Guide to SFTP Download](https://github.com/GSA/IAE-Architecture/blob/master/as-is/tech-docs/SAM/Guide%20to%20Downloading%20SAM%20Extracts%20via%20SFTP%20Site.pdf?raw=true) | Instruction guide on how to download SAM extract files.|
| <a href="https://github.com/GSA/IAE-Architecture/tree/master/as-is/tech-docs/SAM/Sample%20Extract%20Files" target="_blank">Sample Files</a> | Sample files at all data access levels. Samplease are in .xls files and zipped up .dat files. |
| [SAM Functional Data Dictionary](https://github.com/GSA/IAE-Architecture/blob/master/as-is/tech-docs/SAM/SAM%20Functional%20Data%20Dictionary%20v4.0.pdf?raw=true) | Version 4.0  |
|---|---|
| [Exclusions Extract User Guide](https://github.com/GSA/IAE-Architecture/blob/master/as-is/tech-docs/SAM/SAM_Exclusions_Extract_User_Guide.pdf?raw=true)|SAM Exclusions Extract contains a list of all currently open exclusions in SAM|


Comments? Questions?  [Talk to us](https://github.com/GSA/openIAE/issues).
