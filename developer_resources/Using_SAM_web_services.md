---
layout: dev_resources
title: Using the SAM Web Services
nav: using_SAM_web_services
---

### Using SAM Web Services 
SAM offers web services to search for both Entity data and Exclusions data.

**Entity Management data can be searched by:**

* ```DUNSNumber``` (Both DUNS and DUNS + 4)
* ```CAGECode```
* ```taxpayerIdentificationNumber``` (requires addtional access  [Click here](http://gsa.github.io/openIAE/developer_resources/Access_SAM_data.html "Data Access") for more information.)<br>
* ```startDate``` & ```endDate``` (Maximum search time allowed between startDate and endDate is 24 hours.)
* ```registrationStatus```

The web service returns the Entity Management Record in XML format for you to consume into your local application. The Entity Management record has four areas:

* ```coreData```
* ```assertions```
* ```repsAndCerts``` (Representations and Certifications)
* ```POCs```(Points of Contact)

You have to put a "Y" in any one of the above element tags to get a result from the web service.

**EndPoint:** [https://gw.sam.gov/SAMWS/1.0/Entity](https://gw.sam.gov/SAMWS/1.0/Entity)
**WSDL File:** [https://gw.sam.gov/SAMWS/1.0/Entity?wsdl](https://gw.sam.gov/SAMWS/1.0/Entity?wsdl)

Need more help? Click [here](https://github.com/GSA/IAE-Architecture/tree/master/as-is/tech-docs/SAM) for the SAM entity web service management tutorial.

**Exclusions can be searched by:**

* ```Name``` (including Business Name, First/Last Name, Partial Name)
* ```Social Security Number```
* ```Taxpayer Identification Number```
* ```Cage Code```
* ```DUNS``` number.

If there is a match the web service returns the Public Exclusion Record in XML for you to consume into your own system.

**EndPoint:** [https://gw.sam.gov/SAMWS/1.0/ExclusionSearch](https://gw.sam.gov/SAMWS/1.0/ExclusionSearch)

**WSDL File:** [https://gw.sam.gov/SAMWS/1.0/ExclusionSearch?wsdl](https://gw.sam.gov/SAMWS/1.0/ExclusionSearch?wsdl)


### Testing SAM Web Services

| Web Service | Endpoint in Test Environment |
|---|---|
| SAM Entity Management |[https://test.sam.gov/SAMWS/1.0/Entity](https://test.sam.gov/SAMWS/1.0/Entity)|
| SAM Exclusion |[https://test.sam.gov/SAMWS/1.0/ExclusionSearch](https://test.sam.gov/SAMWS/1.0/ExclusionSearch)|



**Test IDs:**

| ID Name | Password | Description | 
|---|---|---|---|
| SAMPublic | Contact IAETransparency@gsa.gov | The public Entity Management Web Service requires authentication |
| SAMFOUO | Contact IAETransparency@gsa.gov | For Official Use Only | 
| SAMSensitive | Contact IAETransparency@gsa.gov | Offers more secure data including banking information and MPIN. |

A test id is not needed for the SAM Exclusions XML web service. There is no role or authentication requirement.
For more information on SAM account access levels click [here](http://gsa.github.io/openIAE/developer_resources/Access_SAM_data.html).
 

**Tools available:**

| Tool Name | Description |
|---|---|
| [Web Services tutorial](https://github.com/GSA/IAE-Architecture/tree/master/as-is/tech-docs/SAM) | Documents how to build an Entity Management web service. Includes various sample request and response for Entity Management. |
| [Web Serivces field mappings](https://github.com/GSA/IAE-Architecture/tree/master/as-is/tech-docs/SAM/SAMWebServicesExtractsMappingsv1.0) | Field and tag mappings for Entity Management Web Services. |
| [Soap UI project for Web Services]() | Project ready for import into Soap UI. Coming Soon! |
| [SAM Functional Data Dictionary](https://github.com/GSA/IAE-Architecture/blob/master/as-is/tech-docs/SAM/SAM%20Functional%20Data%20Dictionary%20v4.0.pdf?raw=true) |All SAM field definitions and enumerations.|
| [Web Services Response Schema Documentation]() | Coming Soon! |

Comments? Questions?  [Talk to us](https://github.com/GSA/openIAE/issues).



