---
layout: dev_resources
nav: access_sam_data
title: Access SAM Data
---
### Access SAM Data

With your SAM account, you can complete a Data Access Request if 
you need to access information of a higher sensitivity level than is 
currently available to you.

• If you want to view data of a higher sensitivity through search, select 
Data Access then click Individual Data Access Request. Complete 
the requested steps.
– For instance, new contracting officers who need EFT information,
would request Entity Management-Sensitive access in SAM.

• If you need to access data Extracts (.csv files) or Web Services (.xml 
downloads), contact the Federal Service Desk at www.fsd.com to 
acquire the necessary forms.

Visit [here](www.fsd.com) to request access to SAM data.

[Quickstart Guide](https://www.sam.gov/sam/transcript/Quick_Guide_for_Federal_Employees.pdf)



#### Updates to SAM Access

Updates to SFTP Access to SAM


Submitted by navinvembar on Monday, July 22, 2013 - 6:12 PM

A week ago, a change was made to the configuration of SAM to address a security concern. 

We had to modify the authentication method for accessing the SAM server via SFTP to utilize only three of the following encryption ciphers: 
aes128-ctr, aes192-ctr, aes256-ctr 

If your SFTP client software does not support the three ciphers above or does support them but is not currently configured to allow SFTP connection using the three ciphers above, you will not be able to properly authenticate with the SAM SFTP server. 

Please verify that your SFTP software is compliant with the above requirement and then try connecting to the SAM SFTP server again. 

If, despite using the correct ciphers, you are still unable to connect to SAM, please contact Navin Vembar (navin.vembar@gsa.gov) and Pam Miller (pamela.miller@gsa.gov) so we can connect you with the technical team to address the issue.
