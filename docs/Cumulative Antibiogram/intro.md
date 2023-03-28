---
sidebar_position: 1
---

# Cumulative Antibiogram

In order to enhance Antimicrobial Stewardship (AMS), the AMS Team needs to know the ongoing susceptibilities within departments, care-types and ultimately on a hospital-wide basis. This is based on culture reports which are then analysed in detail. The same needs to be done for MDROs as well. ZEVAC makes this process a lot easier for the AMS Team by populating the hospital antibiogram and allowing them to have departmental and care type based filtering at the minutest level.

The data for populating hospital antibiograms is imported from hospital’s IT systems, primarily from the Health Management Information System (HMIS) and a Laboratory Information System (LIS). The culture tests are conducted in a hospital’s laboratory and saved on its IT systems which are later imported into the ZEVAC using ETL process. The ETL runs  once in a day (usually around 2 AM in client’s timezone). This data is stored in the zevac_zevacmodel table.

A description of the important data points required for the module is given below: 


Component
Table Name
Variables

Demographic details
zevac_zevacmodel
Patient’s age
 gender




Point of care features
zevac_zevacmodel
Caretype 
Location
Department
Ward
Therapy Type
Admission/Release Details
zevac_zevacmodel
Cause of Admission Admission Date
 Release Date

Culture details
zevac_zevacmodel
Organism found in culture
 Susceptibility
Comorbidities


Figure T1: Important data points required for Hospital Antibiogram 

Once these records are imported into the ZEVAC, the data is pre-processed and then ZEVAC cultivates the Susceptibility Reports for the same based on the infections and bugs as per the Clinical and Laboratory Standards Institute document M39-A4— Analysis and Presentation of Cumulative Antimicrobial Susceptibility Test Data. ZEVAC also produces bug - drug and drug - bug distribution for a particular specimen type. The system allows the user to view the antibiograms for specific time periods, specific departments and specific care types as well. The bugs are grouped into ‘Gram Negative’ and  ‘Gram Positive’. One can also view the prevalence trend for a particular drug or a particular bug for a specific sample type in the Hospital Antibiogram. (See figure b) This can again be filtered on department and care-type level and for a specific time period. ZEVAC is also engineered to show Multi Drug Resistant Organisms (MDROs) and their prevalence trend. In the drug panel (in hospital antibiogram section, see figure b, third leaflet), the drugs are marked along with their associated categories (if any), eg, Drugs falling in PreAuth (Pre-authorisation) category are marked with the "!” sign, which on hovering shows that the particular drug is associated with the PreAuth category. 

ZEVAC also generates susceptibility trends for a drug-bug combination based on the culture reports (see Figure d).