# Dynamics 365 for Finance and Operations Customers integration project
# Dynamics 365 for Finance and Operations Update 7.3, 8.0 and 8.1 fix
# Includes the solution file DMOD365SampleDev.sln
# Model file [DMO D365 Dev]

In Dynamics 365 for Finance and Operations when customers are imported or integrated with external systems there is a flag 
called IsExternallyMaintained that is set to Yes. This flag sets the addresses (primary and non-primary) to non-editable. 

Through this sample code, the user will have the ability to enter non-primary addresses explicitly in Dynamics 365 for Finance and 
Operations. Currently, this is a bug and the user doesn't have the ability to enter non-primary addresses and/or contacts.  
