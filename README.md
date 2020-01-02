# Dynamics 365 for Finance and Operations Customers and Products integration project
# Dynamics 365 for Finance and Operations Update 31
# Includes the solution file DMOD365SampleDev.sln
# Model file [DMO D365 Dev]

In Dynamics 365 for Finance and Operations when customers are imported or integrated with external systems there is a flag 
called IsExternallyMaintained that is set to Yes. This flag sets the addresses (primary and non-primary) to non-editable. 

Through this sample code, the user will have the ability to enter non-primary addresses explicitly in Dynamics 365 for Finance 
and Operations. Currently, this is a bug and the user doesn't have the ability to enter non-primary addresses and/or contacts. 
Once the data flows in through the CustCustomerV3Entity used for data integration, there is a flag called IsExternallyMaintained
that is set to 'Yes'. This flag sets the Address and the contact fields as non-editable (primary and non-primary). The ability for
the user is to enter atleast addresses and contacts that are of that type non-primary. Through this piece of X++ code, the user
can enter non-primary addresses and contacts in Finance and Operations.
