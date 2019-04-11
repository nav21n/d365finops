# Dynamics 365 for Finance and Operations Customers and Products integration project
# Dynamics 365 for Finance and Operations Update 7.3, 8.0 and 8.1 fix
# Includes the solution file DMOD365SampleDev.sln
# Model file [DMO D365 Dev]

In Dynamics 365 for Finance and Operations when customers are imported or integrated with external systems there is a flag 
called IsExternallyMaintained that is set to Yes. This flag sets the addresses (primary and non-primary) to non-editable. 

Through this sample code, the user will have the ability to enter non-primary addresses explicitly in Dynamics 365 for Finance 
and Operations. Currently, this is a bug and users currently don't have the ability to enter non-primary addresses and/or contacts. 
Once the data flows in through the CustCustomerV3Entity used for data integration, there is a flag called IsExternallyMaintained
that is set to 'Yes'. This flag sets the Address and the contact fields as non-editable (primary and non-primary). The ability for
the user is to enter atleast addresses and contacts that are of that type non-primary. Through this piece of X++ code, the user
can enter non-primary addresses and contacts in Finance and Operations.
Note: Code resides in the var layer. 

Projects Used:
DMOD365SampleDev. 

Extensions Used:
#Data Entities:
  CustCustomerV3Entity.DMOSamp

#Staging Table Used:
  CustCustomerV3Staging.DMOSamp

#Event Handler Used:
  DMO_CustTableFrm_EventHandler
  DMO_LogisticsContactInfoFrm_EventHandler
  DMO_LogisticsContactInfoGridFrm_EventHandler
  DMO_LogisticsPostalAddress

Also, through this Dynamics 365 for Finance and Operations project, products from Finance and Operations flow into the product catalogue in Sales. 

Extensions Used:
#Data Entities:
 EcoResSellableReleasedProductsEntity.DMOSamp 
 
#Staging Table Used:
 EcoResSellableReleasedProductStaging.DMOSamp
 InventTable.DMOSamp
 
#Event Handler Used:
 DMO_EcoResSellableProductEntity 
 

  
 
